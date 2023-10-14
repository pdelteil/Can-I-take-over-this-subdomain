
## What tha fork? 

This fork is a legacy version of [Can I take over XYZ?](https://github.com/EdOverflow/can-i-take-over-xyz)

This repo will be updated faster and better. 

## What is a subdomain takeover?

> Subdomain takeover vulnerabilities occur when a subdomain (subdomain.example.com) is pointing to a service (e.g. GitHub pages, Heroku, etc.) that has been removed or deleted. This allows an attacker to set up a page on the service that was being used and point their page to that subdomain. 

You can read up more about subdomain takeovers here:

- <https://0xpatrik.com/subdomain-takeover-ns/>

## Fingerprints and Nuclei templates

The only tool that will be supporting the discovery of takeover is going to be Nuclei (takeover -> template)


## How to contribute

1. You can submit new services [here](https://github.com/pdelteil/can-i-take-over-this-subdomain/issues/new/choose).
2. You can add the service directly in this [Readme](https://github.com/pdelteil/Can-I-take-over-this-subdomain/edit/master/README.md)
3. Create a Nuclei template for takeovers. (Doesn't matter if it's not vulnerable anymore).
4. Find public bug bounty reports and link it to the takeover.
5. Sponsore this project. 

# All entries

Fingerprints are found in the linked issues or in the nuclei templates. 

Service|Vulnerable|Fingerprint|Discussions|Docs|Nuclei template
:---|:---:|:---:|:---:|:---:|:---:
[Acquia](https://www.acquia.com/)|No||[:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/103)||:x:
[Agile CRM](https://www.agilecrm.com/)|Yes||[:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/145)||[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/agilecrm-takeover.yaml)
[Airee.ru](https://айри.рф/)|Yes||[:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/104)||[:heavy_check_mark: ](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/airee-takeover.yaml)
Anima|Yes||[:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/126)|[:blue_book:](https://docs.animaapp.com/v1/launchpad/08-custom-domain.html)| [:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/anima-takeover.yaml)
Akamai|No||[:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/13) |
AWS EC2|Yes||[:information_source:](https://github.com/pdelteil/Can-I-take-over-this-subdomain/discussions/3)||[:heavy_check_mark: ](https://github.com/projectdiscovery/nuclei-templates/blob/main/dns/ec2-detection.yaml)
AWS Elastic Beanstalk|Yes||[:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/194)||[:heavy_check_mark: ](https://github.com/projectdiscovery/nuclei-templates/blob/main/dns/elasticbeanstalk-takeover.yaml)
AWS Load Balancer (ELB)|Yes|| [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/137)||
AWS S3|Yes||[:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/36)||[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/aws-bucket-takeover.yaml)
Azure|Edge case|| [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/35) ||[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/dns/azure-takeover-detection.yaml)
Bitbucket|Yes||||[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/bitbucket-takeover.yaml)
Campaign Monitor|Yes||[:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/275)|[:blue_book:](https://help.campaignmonitor.com/custom-domain-names)|[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/campaignmonitor-takeover.yaml)
Cargo Collective|Yes||[:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/152)| [:blue_book:](https://support.2.cargocollective.com/Using-a-Third-Party-Domain)||[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/cargocollective-takeover.yaml)
Cloudfront|No| ViewerCertificateException| [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/29) | [:blue_book:](https://aws.amazon.com/blogs/networking-and-content-delivery/continually-enhancing-domain-security-on-amazon-cloudfront/)
Desk|No|`Please try again or try Desk.com free for 14 days.`| [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/9)
Digital Ocean |Yes| Domain uses DO name servers with no records in DO. |   |   |
Discourse |Yes| | | [:closed_book:](https://hackerone.com/reports/264494)
Fastly|No| `Fastly error: unknown domain:`| [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/22)
Feedpress|No| `The feed has not been found.`| [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/80)
Firebase |No| | [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/128) |
Fly.io|Yes| `404 Not Found`| [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/101)
Freshdesk|No|`We couldn't find servicedesk.victim.tld Maybe this is still fresh! You can claim it now at http://www.freshservice.com/signup`| [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/214)| [:blue_book:](https://support.freshdesk.com/support/solutions/articles/37590-using-a-vanity-support-url-and-pointing-the-cname)
Frontify | Edge case | `404 - Page Not Found` `Oops… looks like you got lost` | [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/170) | 
Gemfury |Yes| | [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/154) | [:green_book:](https://khaledibnalwalid.wordpress.com/2020/06/25/gemfury-subdomain-takeover/)|[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/gemfury-takeover.yaml)
Ghost|Yes| `The thing you were looking for is no longer here, or never was`|
Gitbook|Yes|| [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/259)||[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/gitbook-takeover.yaml)
Github| Edge case|| [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/37) [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/68)||[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/github-takeover.yaml)
Gitlab|No|| |[:closed_book:](https://hackerone.com/reports/312118)
Google Cloud Storage |No|<?xml version='1.0' encoding='UTF-8'?><Error><Code>NoSuchBucket</Code><Message>The specified bucket does not exist.</Message></Error>   
Google Sites|No|`The requested URL was not found on this server. That’s all we know.`                                                    | [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/277) |[:blue_book:](https://support.google.com/webmasters/answer/9008080?visit_id=637981741431097680-3818919062&rd=2)|
HatenaBlog |Yes||||[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/hatenablog-takeover.yaml)
Help Juice|Yes||| [:blue_book:](https://help.helpjuice.com/en_US/using-your-custom-domain/how-to-set-up-a-custom-domain)|[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/helpjuice-takeover.yaml)
Help Scout|Yes||| [:blue_book:](https://docs.helpscout.net/article/42-setup-custom-domain)|[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/helpscout-takeover.yaml)
Heroku| Edge case| `No such app`| [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/38)
HubSpot|No|`This page isn’t available`
Instapage |No| | [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/73) | |
Intercom|Yes| `Uh oh. That page doesn't exist.`| [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/69) | [:blue_book:](https://www.intercom.com/help/)
JetBrains|Yes| `is not a registered InCloud YouTrack`| | [:blue_book:](https://www.jetbrains.com/help/youtrack/incloud/Domain-Settings.html)
Key CDN|No| | [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/112) |
Kinsta|Yes| `No Site For Domain`|[:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/48) | [:blue_book:](https://kinsta.com/knowledgebase/add-domain/)
Landingi  | Edge case| `It looks like you’re lost...` | [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/117)
LaunchRock|Yes||[:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/74) | |[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/launchrock-takeover.yaml)
Mashery|Edge Case||[:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/14)| [:closed_book:](https://hackerone.com/reports/275714) | [:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/mashery-takeover.yaml)
Medium| Edge Case | ``Oops! We couldn’t find that page. Sorry about that.``| [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/206)| [:closed_book:](https://hackerone.com/reports/1034023) 
Netlify | Edge Case | `Not Found - Request ID:`| [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/40) |
Ngrok |Yes|`Tunnel *.ngrok.io not found` | [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/92) | [:blue_book:](https://ngrok.com/docs#http-custom-domains)
Pantheon|Yes||[:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/24) | [:orange_book:](https://medium.com/@hussain_0x3c/hostile-subdomain-takeover-using-pantheon-ebf4ab813111)| [:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/pantheon-takeover.yaml)
Pingdom |Yes| `Sorry, couldn't find the status page` | [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/144) | [:blue_book:](https://help.pingdom.com/hc/en-us/articles/205386171-Public-Status-Page)
Readme.io |Yes| `Project doesnt exist... yet!` | [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/41)
Sendgrid|No|                                                                         |
Shopify| Edge Case||[:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/32) [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/46)| [:orange_book:](https://medium.com/@thebuckhacker/how-to-do-55-000-subdomain-takeover-in-a-blink-of-an-eye-a94954c3fc75) |[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/shopify-takeover.yaml)
Short.io|Yes||[:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/260)||[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/short-io.yaml)
SmartJobBoard|Yes||[:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/139) | [:blue_book:](https://help.smartjobboard.com/en/articles/1269655-connecting-a-custom-domain-name)|[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/smartjob-takeover.yaml)
Smartling| Edge Case|`Domain is not configured`  | [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/67)
Squarespace|No|                                                                         |
Statuspage |No| | [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/pull/105) [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/pull/171) | [:blue_book:](https://help.statuspage.io/knowledge_base/topics/domain-ownership) [:blue_book:](https://support.atlassian.com/statuspage/docs/configure-your-dns/) |[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/commit/b59915c4aee18e04d2680ef32fdfa88f1e725b6f#diff-03ac5eecfcef771523f7758b50e75ab5ca1e2eb0b9f5bf6779a18f8c98e6aba3)
Strikingly|Yes||[:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/58) | [:orange_book:](https://medium.com/@sherif0x00/takeover-subdomains-pointing-to-strikingly-5e67df80cdfd)| [:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/strikingly-takeover.yaml)
Surge.sh|Yes| `project not found`|| [:blue_book:](https://surge.sh/help/adding-a-custom-domain)
Surveygizmo|Yes||||[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/surveygizmo-takeover.yaml)
SurveySparrow |Yes| `'Ouch! Account not found'` | [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/281) |[:blue_book:]( https://help.surveysparrow.com/custom-domain)
TeamWork |Yes| | || [:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/teamwork-takeover.yaml)
Tumblr| Edge Case||[:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/240) | [:blue_book:](https://www.tumblr.com/docs/en/custom_domains)|[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/tumblr-takeover.yaml)
Tilda| Edge Case | `Please renew your subscription`| [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/155)[:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/pull/20)
Uberflip|Yes|| [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/150) | [:blue_book:](https://help.uberflip.com/hc/en-us/articles/360018786372-Custom-Domain-Set-up-Your-Hub-on-a-Subdomain)|[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/uberflip-takeover.yaml)
Unbounce|No||[:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/11)||[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/1dc592a59a0ff9729df00ce2de007f8ba0b38bf5/takeovers/unbounce-takeover.yaml) 
Uptimerobot|Yes||[:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/45) | [:orange_book:](https://exploit.linuxsec.org/uptimerobot-com-custom-domain-subdomain-takeover/)|[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/uptimerobot-takeover.yaml)
UserVoice|Yes| |||[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/uservoice-takeover.yaml)
Vercel|No| |[:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/183)||[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/vercel-takeover.yaml)
Webflow| Edge Case| |[:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/44) |[:blue_book:](https://forum.webflow.com/t/hosting-a-subdomain-on-webflow/59201)|[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/webflow-takeover.yaml)
Wix| Edge Case||[:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/231) | | [:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/wix-takeover.yaml)
Wordpress|Yes|| [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/pull/176)||[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/wordpress-takeover.yaml)
Worksites |Yes| `Hello! Sorry, but the website you&rsquo;re looking for doesn&rsquo;t exist.` | [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/142) | 
WP Engine|No||
Zendesk|No|`Help Center Closed`| [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/23) | [:blue_book:](https://support.zendesk.com/hc/en-us/articles/203664356-Changing-the-address-of-your-Help-Center-subdomain-host-mapping-)

# Stats 
| Total Takeovers | Active Takeovers | Inactive Takeovers | Edge Case Takeovers | 
   |------------------|-------------------|--------------------|---------------------| 
  | 74 | 39 | 21 | 14 | 

