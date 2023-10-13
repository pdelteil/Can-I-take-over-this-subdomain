
## What tha fork? 

This fork is a legacy version of [Can I take over XYZ?](https://github.com/EdOverflow/can-i-take-over-xyz)
This repo will be updated faster and in a clearer manner. 



## What is a subdomain takeover?

> Subdomain takeover vulnerabilities occur when a subdomain (subdomain.example.com) is pointing to a service (e.g. GitHub pages, Heroku, etc.) that has been removed or deleted. This allows an attacker to set up a page on the service that was being used and point their page to that subdomain. 

You can read up more about subdomain takeovers here:

- <https://0xpatrik.com/subdomain-takeover-ns/>

## Fingerprints and Nuclei templates

The only tool that will be supporting the discovery of takeover is going to be Nuclei (takeover -> template)


## How to contribute

You can submit new services [here](https://github.com/pdelteil/can-i-take-over-this-subdomain/issues/new/choose).


# All entries

Fingerprints are found in the linked issues or in the nuclei templates. 

Engine                                        | Vulnerable?         | Fingerprint                                                             | Discussion                                                    | Documentation | Nuclei template 
--------------------------------------------- | -------------- | ----------------------------------------------------------------------- | ------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------|-----------------
Acquia|No||[Issue #103](https://github.com/EdOverflow/can-i-take-over-xyz/issues/103)||No
Agile CRM|Yes||[Issue #145](https://github.com/EdOverflow/can-i-take-over-xyz/issues/145)||[Yes](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/agilecrm-takeover.yaml)
Airee.ru|Yes||[Issue #104](https://github.com/EdOverflow/can-i-take-over-xyz/issues/104)||[Yes](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/airee-takeover.yaml)
Anima | Yes ||[Issue #126](https://github.com/EdOverflow/can-i-take-over-xyz/issues/126)|[Anima Documentation](https://docs.animaapp.com/v1/launchpad/08-custom-domain.html)| [Yes](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/anima-takeover.yaml)
Akamai|No||[Issue #13](https://github.com/EdOverflow/can-i-take-over-xyz/issues/13) |
AWS S3|Yes||[Issue #36](https://github.com/EdOverflow/can-i-take-over-xyz/issues/36)||[Yes](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/aws-bucket-takeover.yaml)
AWS Load Balancer (ELB)|No| status NXDOMAIN and CNAME pointing to XYZ.elb.amazonaws.com| [Issue #137](https://github.com/EdOverflow/can-i-take-over-xyz/issues/137)
AWS/Elastic Beanstalk|Yes|`404 Not Found`|[Issue #194](https://github.com/EdOverflow/can-i-take-over-xyz/issues/194)
Azure | Edge case | | [Issue #35](https://github.com/EdOverflow/can-i-take-over-xyz/issues/35) ||[Yes](https://github.com/projectdiscovery/nuclei-templates/blob/main/dns/azure-takeover-detection.yaml)
Bitbucket|Yes||||[Yes](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/bitbucket-takeover.yaml)
Campaign Monitor| Yes||[Issue #275](https://github.com/EdOverflow/can-i-take-over-xyz/issues/275)|[Support Page](https://help.campaignmonitor.com/custom-domain-names)|[Yes](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/campaignmonitor-takeover.yaml)
Cargo Collective|Yes||[Issue #152](https://github.com/EdOverflow/can-i-take-over-xyz/issues/152)| [Cargo Support Page](https://support.2.cargocollective.com/Using-a-Third-Party-Domain)||[Yes](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/cargocollective-takeover.yaml)
Cloudfront| No| ViewerCertificateException| [Issue #29](https://github.com/EdOverflow/can-i-take-over-xyz/issues/29) | [Domain Security on Amazon CloudFront](https://aws.amazon.com/blogs/networking-and-content-delivery/continually-enhancing-domain-security-on-amazon-cloudfront/)
Desk|No|`Please try again or try Desk.com free for 14 days.`| [Issue #9](https://github.com/EdOverflow/can-i-take-over-xyz/issues/9)
Digital Ocean | Yes | Domain uses DO name servers with no records in DO. |   |   |
Discourse | Yes | | | [Hackerone](https://hackerone.com/reports/264494)
Fastly| No| `Fastly error: unknown domain:`| [Issue #22](https://github.com/EdOverflow/can-i-take-over-xyz/issues/22)
Feedpress| No| `The feed has not been found.`| [Issue #80](https://github.com/EdOverflow/can-i-take-over-xyz/issues/80)
Firebase | No | | [Issue #128](https://github.com/EdOverflow/can-i-take-over-xyz/issues/128) |
Fly.io| Yes| `404 Not Found`| [Issue #101](https://github.com/EdOverflow/can-i-take-over-xyz/issues/101)
Freshdesk| No |`We couldn't find servicedesk.victim.tld Maybe this is still fresh! You can claim it now at http://www.freshservice.com/signup`| [Issue #214](https://github.com/EdOverflow/can-i-take-over-xyz/issues/214)| [Freshdesk Support Page](https://support.freshdesk.com/support/solutions/articles/37590-using-a-vanity-support-url-and-pointing-the-cname)
Frontify | Edge case | `404 - Page Not Found` `Oops… looks like you got lost` | [Issue #170](https://github.com/EdOverflow/can-i-take-over-xyz/issues/170) | 
Gemfury | Yes | `404: This page could not be found.` | [Issue #154](https://github.com/EdOverflow/can-i-take-over-xyz/issues/154) | [Article](https://khaledibnalwalid.wordpress.com/2020/06/25/gemfury-subdomain-takeover/)
Ghost| Yes| `The thing you were looking for is no longer here, or never was`|
Github| Edge case|| [Issue #37](https://github.com/EdOverflow/can-i-take-over-xyz/issues/37) [Issue #68](https://github.com/EdOverflow/can-i-take-over-xyz/issues/68)||[Yes](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/github-takeover.yaml)
Gitlab| No || [HackerOne #312118](https://hackerone.com/reports/312118)
Google Cloud Storage | No |   <?xml version='1.0' encoding='UTF-8'?><Error><Code>NoSuchBucket</Code><Message>The specified bucket does not exist.</Message></Error>   
Google Sites| No| `The requested URL was not found on this server. That’s all we know.`                                                    | [Issue #277](https://github.com/EdOverflow/can-i-take-over-xyz/issues/277) | [Google Support](https://support.google.com/webmasters/answer/9008080?visit_id=637981741431097680-3818919062&rd=2)|
HatenaBlog | vulnerable | `404 Blog is not found`|
Help Juice| Yes| `We could not find what you're looking for.`|| [Help Juice Support Page](https://help.helpjuice.com/en_US/using-your-custom-domain/how-to-set-up-a-custom-domain)
Help Scout| Yes| `No settings were found for this company:`|| [HelpScout Docs](https://docs.helpscout.net/article/42-setup-custom-domain)
Heroku| Edge case| `No such app`| [Issue #38](https://github.com/EdOverflow/can-i-take-over-xyz/issues/38)
HubSpot| No | `This page isn’t available`
Instapage | No | | [Issue #73](https://github.com/EdOverflow/can-i-take-over-xyz/issues/73) | |
Intercom| Yes| `Uh oh. That page doesn't exist.`| [Issue #69](https://github.com/EdOverflow/can-i-take-over-xyz/issues/69) | [Help center](https://www.intercom.com/help/)
JetBrains| Yes| `is not a registered InCloud YouTrack`| | [YouTrack InCloud Help Page](https://www.jetbrains.com/help/youtrack/incloud/Domain-Settings.html)
Key CDN| No| | [Issue #112](https://github.com/EdOverflow/can-i-take-over-xyz/issues/112) |
Kinsta| Yes| `No Site For Domain`|[Issue #48](https://github.com/EdOverflow/can-i-take-over-xyz/issues/48) | [kinsta-add-domain](https://kinsta.com/knowledgebase/add-domain/)
Landingi  | Edge case| `It looks like you’re lost...` | [Issue #117](https://github.com/EdOverflow/can-i-take-over-xyz/issues/117)
LaunchRock| Yes||[Issue #74](https://github.com/EdOverflow/can-i-take-over-xyz/issues/74) | |[Yes](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/launchrock-takeover.yaml)
Mashery| Edge Case | `Unrecognized domain`| [HackerOne #275714](https://hackerone.com/reports/275714), [Issue #14](https://github.com/EdOverflow/can-i-take-over-xyz/issues/14)
Medium| Edge Case | ``Oops! We couldn’t find that page. Sorry about that.``| [Issue #206](https://github.com/EdOverflow/can-i-take-over-xyz/issues/206)| [HackerOne](https://hackerone.com/reports/1034023) 
Netlify | Edge Case | `Not Found - Request ID:`| [Issue #40](https://github.com/EdOverflow/can-i-take-over-xyz/issues/40) |
Ngrok | Yes |`Tunnel *.ngrok.io not found` | [Issue #92](https://github.com/EdOverflow/can-i-take-over-xyz/issues/92) | [Ngrok Documentation](https://ngrok.com/docs#http-custom-domains)
Pantheon| Yes| `404 error unknown site!`|[Issue #24](https://github.com/EdOverflow/can-i-take-over-xyz/issues/24) | [Pantheon-Sub-takeover](https://medium.com/@hussain_0x3c/hostile-subdomain-takeover-using-pantheon-ebf4ab813111)
Pingdom | Yes | `Sorry, couldn't find the status page` | [Issue #144](https://github.com/EdOverflow/can-i-take-over-xyz/issues/144) | [Support Page](https://help.pingdom.com/hc/en-us/articles/205386171-Public-Status-Page)
Readme.io | Yes | `Project doesnt exist... yet!` | [Issue #41](https://github.com/EdOverflow/can-i-take-over-xyz/issues/41)
Sendgrid| No|                                                                         |
Shopify| Edge Case| `Sorry, this shop is currently unavailable.`|[Issue #32](https://github.com/EdOverflow/can-i-take-over-xyz/issues/32), [Issue #46](https://github.com/EdOverflow/can-i-take-over-xyz/issues/46)| [Medium Article](https://medium.com/@thebuckhacker/how-to-do-55-000-subdomain-takeover-in-a-blink-of-an-eye-a94954c3fc75) 
Short.io | Yes| `Link does not exist` | [Issue #260](https://github.com/EdOverflow/can-i-take-over-xyz/issues/260)
SmartJobBoard | Yes | `This job board website is either expired or its domain name is invalid.` | [Issue #139](https://github.com/EdOverflow/can-i-take-over-xyz/issues/139) | [Support Page](https://help.smartjobboard.com/en/articles/1269655-connecting-a-custom-domain-name)
Smartling| Edge Case|`Domain is not configured`  | [Issue #67](https://github.com/EdOverflow/can-i-take-over-xyz/issues/67)
Squarespace| No |                                                                         |
Statuspage | No | `Status page pushed a DNS verification in order to prevent malicious takeovers what they mentioned in` [This Doc](https://support.atlassian.com/statuspage/docs/configure-your-dns/) | [PR #105](https://github.com/EdOverflow/can-i-take-over-xyz/pull/105) and [PR #171](https://github.com/EdOverflow/can-i-take-over-xyz/pull/171) | [Statuspage documentation](https://help.statuspage.io/knowledge_base/topics/domain-ownership) |          
Strikingly| Yes| `page not found`|[Issue #58](https://github.com/EdOverflow/can-i-take-over-xyz/issues/58) | [Strikingly-Sub-takeover](https://medium.com/@sherif0x00/takeover-subdomains-pointing-to-strikingly-5e67df80cdfd)
Surge.sh| Yes| `project not found`|| [Surge Documentation](https://surge.sh/help/adding-a-custom-domain)
SurveySparrow | Yes | `'Ouch! Account not found'` | [Issue #281](https://github.com/EdOverflow/can-i-take-over-xyz/issues/281) |[Custom domain]( https://help.surveysparrow.com/custom-domain)
Tumblr| Edge Case| `Whatever you were looking for doesn't currently exist at this address` | [Issue #240](https://github.com/EdOverflow/can-i-take-over-xyz/issues/240) | [Tumblr Custom Domains](https://www.tumblr.com/docs/en/custom_domains)
Tilda| Edge Case | `Please renew your subscription`| [Issue #155](https://github.com/EdOverflow/can-i-take-over-xyz/issues/155)[PR #20](https://github.com/EdOverflow/can-i-take-over-xyz/pull/20)
Uberflip | Yes | `Non-hub domain, The URL you've accessed does not provide a hub.` | [Issue #150](https://github.com/EdOverflow/can-i-take-over-xyz/issues/150) | [Uberflip Documentation](https://help.uberflip.com/hc/en-us/articles/360018786372-Custom-Domain-Set-up-Your-Hub-on-a-Subdomain)
Unbounce| No | `The requested URL was not found on this server.`| [Issue #11](https://github.com/EdOverflow/can-i-take-over-xyz/issues/11)||[Yes](https://github.com/projectdiscovery/nuclei-templates/blob/1dc592a59a0ff9729df00ce2de007f8ba0b38bf5/takeovers/unbounce-takeover.yaml) 
Uptimerobot| Yes| `page not found`|[Issue #45](https://github.com/EdOverflow/can-i-take-over-xyz/issues/45) | [Uptimerobot-Sub-takeover](https://exploit.linuxsec.org/uptimerobot-com-custom-domain-subdomain-takeover/)
UserVoice| Yes| `This UserVoice subdomain is currently available!`                      |
Vercel| No| |[Issue #183](https://github.com/EdOverflow/can-i-take-over-xyz/issues/183)||[Yes](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/vercel-takeover.yaml)
Webflow| Edge Case| |[Issue #44](https://github.com/EdOverflow/can-i-take-over-xyz/issues/44) |[forum webflow](https://forum.webflow.com/t/hosting-a-subdomain-on-webflow/59201)|[Yes](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/webflow-takeover.yaml)
Wix| Edge Case||[Issue #231](https://github.com/EdOverflow/can-i-take-over-xyz/issues/231) | | [Yes](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/wix-takeover.yaml)
Wordpress| Yes| `Do you want to register *.wordpress.com?`| [PR #176](https://github.com/EdOverflow/can-i-take-over-xyz/pull/176)|
Worksites | Yes | `Hello! Sorry, but the website you&rsquo;re looking for doesn&rsquo;t exist.` | [Issue #142](https://github.com/EdOverflow/can-i-take-over-xyz/issues/142) | 
WP Engine| No ||
Zendesk| No|`Help Center Closed`| [Issue #23](https://github.com/EdOverflow/can-i-take-over-xyz/issues/23) | [Zendesk Support](https://support.zendesk.com/hc/en-us/articles/203664356-Changing-the-address-of-your-Help-Center-subdomain-host-mapping-)
