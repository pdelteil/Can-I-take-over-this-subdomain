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
5. Sponsor this project. 

# All entries

Fingerprints are found in the linked issues or in the nuclei templates. 

Service|Vulnerable|Discussions|Docs|Nuclei template
:---|:---:|:---:|:---:|:---:
[Acquia](https://www.acquia.com/)|No|[:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/103)||[:heavy_check_mark:](https://github.com/rtcms/nuclei-templates/blob/fc5546e4720adaa026a74b5937f474cc10c14f22/takeovers/acquia-takeover.yaml)
Aftership|Yes|[:information_source:](https://github.com/pdelteil/Can-I-take-over-this-subdomain/discussions/8)||[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/aftership-takeover.yaml)
[Agile CRM](https://www.agilecrm.com/)|Yes|[:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/145)||[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/agilecrm-takeover.yaml)
Aha|Yes|[:information_source:](https://github.com/pdelteil/Can-I-take-over-this-subdomain/discussions/9)||[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/aha-takeover.yaml)
[Airee.ru](https://айри.рф/)|Yes|[:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/104)||[:heavy_check_mark: ](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/airee-takeover.yaml)
Anima|Yes|[:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/126)|[:blue_book:](https://docs.animaapp.com/v1/launchpad/08-custom-domain.html)| [:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/anima-takeover.yaml)
Announcekit|Yes|[:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/228)||[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/announcekit-takeover.yaml)
Akamai|No|[:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/13) ||:x:
AWS Cognito | Yes|[:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/358)||:x:
AWS EC2|Yes|[:information_source:](https://github.com/pdelteil/Can-I-take-over-this-subdomain/discussions/3)||[:heavy_check_mark: ](https://github.com/projectdiscovery/nuclei-templates/blob/main/dns/ec2-detection.yaml)
AWS Elastic Beanstalk|Yes|[:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/194)||[:heavy_check_mark: ](https://github.com/projectdiscovery/nuclei-templates/blob/main/dns/elasticbeanstalk-takeover.yaml)
AWS Load Balancer (ELB)|Yes| [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/137)||:x:
AWS S3|Yes|[:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/36)||[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/aws-bucket-takeover.yaml)
Azure|Edge case| [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/35) ||[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/dns/azure-takeover-detection.yaml)
BetterUptime|Yes|[:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/368)||[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/63427f8332a0c0174b4c6e35d6a70a649b3304e9/http/takeovers/betteruptime-takeover.yaml)
Bigcartel|Yes|||[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/bigcartel-takeover.yaml)
Bitbucket|Yes|||[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/bitbucket-takeover.yaml)
Campaign Monitor|Yes|[:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/275)|[:blue_book:](https://help.campaignmonitor.com/custom-domain-names)|[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/campaignmonitor-takeover.yaml)
Cargo Collective|Yes|[:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/152)| [:blue_book:](https://support.2.cargocollective.com/Using-a-Third-Party-Domain)|:x:
Clever|Yes|||[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/clever-takeover.yaml)
Cloudfront|No| [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/29) | [:blue_book:](https://aws.amazon.com/blogs/networking-and-content-delivery/continually-enhancing-domain-security-on-amazon-cloudfront/)|:x:
Desk|No| [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/9)||:x:
Digital Ocean |Yes|   |   |:x:
Discourse |Yes| | [:closed_book:](https://hackerone.com/reports/264494)|:x:
[Fastly](https://www.fastly.com/)|No| [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/22)||[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/e254f7b884dc975316a2f8d77e3fe0ce140cc91b/takeovers/fastly-takeover.yaml)
Feedpress|No| [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/80)||:x:
Firebase |No| [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/128) ||:x:
Flexbe |Yes| [:information_source:](https://web.archive.org/web/20211002185648/https://github.com/EdOverflow/can-i-take-over-xyz/issues/237) ||[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/flexbe-takeover.yaml)
Fly.io|Yes| [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/132)|[:closed_book:](https://hackerone.com/reports/576857)|[:heavy_check_mark:](https://github.com/pdelteil/Can-I-take-over-this-subdomain/blob/master/templates/fly-io.yaml)
Freshdesk|No| [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/214)| [:blue_book:](https://support.freshdesk.com/support/solutions/articles/37590-using-a-vanity-support-url-and-pointing-the-cname)|:x:
Frontify |Edge case|[:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/170) || [:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/frontify-takeover.yaml)|:x:
Gemfury |Yes| [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/154) | [:green_book:](https://khaledibnalwalid.wordpress.com/2020/06/25/gemfury-subdomain-takeover/)|[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/gemfury-takeover.yaml)
Ghost|Yes|[:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/8)||[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/ghost-takeover.yaml)
Gitbook|Yes| [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/259)||[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/gitbook-takeover.yaml)
Github| Edge case| [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/37) [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/68)||[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/github-takeover.yaml)
Gitlab|No| |[:closed_book:](https://hackerone.com/reports/312118)|:x:
Gohire|Yes|[:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/403)||[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/dc4019ff0ce089802a84ff4f12190b2ab5fa96dc/http/takeovers/gohire-takeover.yaml)
Google Cloud Storage |No|[:information_source:](https://github.com/pdelteil/Can-I-take-over-this-subdomain/discussions/7)||[:heavy_check_mark:](https://github.com/pdelteil/Can-I-take-over-this-subdomain/blob/master/templates/gbucket.yaml)
Google Sites|No| [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/277) |[:blue_book:](https://support.google.com/webmasters/answer/9008080?visit_id=637981741431097680-3818919062&rd=2)|[:heavy_check_mark:](https://github.com/pdelteil/Can-I-take-over-this-subdomain/blob/master/templates/googlesites-takeover.yaml)
HatenaBlog |Yes|||[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/hatenablog-takeover.yaml)
[HelpDocs](https://www.helpdocs.io/)|Yes|||[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/helpdocs-takeover.yaml)
Help Juice|Yes|| [:blue_book:](https://help.helpjuice.com/en_US/using-your-custom-domain/how-to-set-up-a-custom-domain)|[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/helpjuice-takeover.yaml)
Help Scout|Yes|| [:blue_book:](https://docs.helpscout.net/article/42-setup-custom-domain)|[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/helpscout-takeover.yaml)
Heroku| Edge case| [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/38)||[:heavy_check_mark:](https://github.com/mosesrenegade/nuclei-templates/blob/75a8c562a3c637a6112aaa522950b512cab09144/http/takeovers/heroku-takeover.yaml)
HubSpot|No|||[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/hubspot-takeover.yaml)
Instapage |No| [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/73) | |:x:
Intercom|Yes| [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/69) | [:blue_book:](https://www.intercom.com/help/)|:x:
JazzHr|No|||[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/jazzhr-takeover.yaml)
JetBrains|Yes||[:blue_book:](https://www.jetbrains.com/help/youtrack/incloud/Domain-Settings.html)|[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/jetbrains-takeover.yaml)
Key CDN|No| [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/112) ||:x:
Kinsta|Yes|[:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/48) | [:blue_book:](https://kinsta.com/knowledgebase/add-domain/)|:x:
Landingi  | Edge case| [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/117)||:x:
LaunchRock|Yes|[:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/74) | |[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/launchrock-takeover.yaml)
LemList|Edge case| ||[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/lemlist-takeover.yaml)
Mashery|Edge Case|[:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/14)| [:closed_book:](https://hackerone.com/reports/275714) | [:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/mashery-takeover.yaml)
Medium| Edge Case | [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/206)| [:closed_book:](https://hackerone.com/reports/1034023) | [:heavy_check_mark:](https://raw.githubusercontent.com/rtcms/nuclei-templates/fc5546e4720adaa026a74b5937f474cc10c14f22/takeovers/medium-takeover.yaml)
Netlify | Edge Case | [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/40) |[:green_book:](https://monish-basaniwal.medium.com/how-i-found-my-first-subdomain-takeover-vulnerability-b7d5c17b61fd)|[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/netlify-takeover.yaml)
Ngrok |Yes| [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/92) | [:blue_book:](https://ngrok.com/docs#http-custom-domains)| [:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/ngrok-takeover.yaml)
Pantheon|Yes|[:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/24) | [:orange_book:](https://medium.com/@hussain_0x3c/hostile-subdomain-takeover-using-pantheon-ebf4ab813111)| [:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/pantheon-takeover.yaml)
Pingdom |Yes|[:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/144) | [:blue_book:](https://help.pingdom.com/hc/en-us/articles/205386171-Public-Status-Page)|[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/pingdom-takeover.yaml)
Readme.io |Yes| [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/41)||[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/edit/main/http/takeovers/readme-takeover.yaml)
Sendgrid|No|||:x:
Shopify| Edge Case|[:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/32) [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/46)| [:orange_book:](https://medium.com/@thebuckhacker/how-to-do-55-000-subdomain-takeover-in-a-blink-of-an-eye-a94954c3fc75) |[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/shopify-takeover.yaml)
Short.io|Yes|[:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/260)||[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/short-io.yaml)
SmartJobBoard|Yes|[:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/139) | [:blue_book:](https://help.smartjobboard.com/en/articles/1269655-connecting-a-custom-domain-name)|[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/smartjob-takeover.yaml)
Smartling| Edge Case| [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/67)||:x:
[Softr.io](https://www.softr.io/)|Yes|[:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/352)|[:blue_book:](https://docs.softr.io/custom-domain-and-publishing/9qTmU2Lj8Gnpr1Ue6dEAkX/add-a-custom-domain-to-your-app/93K5bLJN3n91MRo9uRGdAf)|[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/e36e3b8c6caffd0f5ff75f3de1e6df30618b02f2/http/takeovers/softr-takeover.yaml)
Squarespace|No|||:x:
[Squadcast](https://www.squadcast.com/)|Yes|||[:heavy_check_mark:](https://github.com/pdelteil/Can-I-take-over-this-subdomain/blob/master/templates/squadcast-takeover.yaml)
Statuspage |No| [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/pull/105) [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/pull/171) | [:blue_book:](https://help.statuspage.io/knowledge_base/topics/domain-ownership) [:blue_book:](https://support.atlassian.com/statuspage/docs/configure-your-dns/) |[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/commit/b59915c4aee18e04d2680ef32fdfa88f1e725b6f#diff-03ac5eecfcef771523f7758b50e75ab5ca1e2eb0b9f5bf6779a18f8c98e6aba3)
Strikingly|Yes|[:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/58) | [:orange_book:](https://medium.com/@sherif0x00/takeover-subdomains-pointing-to-strikingly-5e67df80cdfd)| [:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/strikingly-takeover.yaml)
[Surge.sh](https://surge.sh/)|Yes|| [:blue_book:](https://surge.sh/help/adding-a-custom-domain)|:x:
Surveygizmo|Yes|||[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/surveygizmo-takeover.yaml)
SurveySparrow |Yes| [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/281) |[:blue_book:]( https://help.surveysparrow.com/custom-domain)|[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/surveysparrow-takeover.yaml)
Tally|Edge Case|[:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/363)||:x:
TeamWork |Yes| || [:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/teamwork-takeover.yaml)
Tumblr| Edge Case|[:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/240) | [:blue_book:](https://www.tumblr.com/docs/en/custom_domains)|[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/tumblr-takeover.yaml)
Tilda| Edge Case | [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/155)[:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/pull/20)||[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/076aa6cafde57ffd2e8781650525122f452e2338/http/takeovers/tilda-takeover.yaml#L4)
Uberflip|Yes| [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/150) | [:blue_book:](https://help.uberflip.com/hc/en-us/articles/360018786372-Custom-Domain-Set-up-Your-Hub-on-a-Subdomain)|[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/uberflip-takeover.yaml)
Unbounce|Edge Case|[:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/11)||[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/1dc592a59a0ff9729df00ce2de007f8ba0b38bf5/takeovers/unbounce-takeover.yaml) 
Uptimerobot|Yes|[:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/45) | [:orange_book:](https://exploit.linuxsec.org/uptimerobot-com-custom-domain-subdomain-takeover/)|[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/uptimerobot-takeover.yaml)
UserResponse|Yes|[:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/357)||:x:
UserVoice|Yes|||[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/uservoice-takeover.yaml)
Vercel|No|[:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/183)||[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/vercel-takeover.yaml)
Webflow| Edge Case|[:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/44) |[:blue_book:](https://forum.webflow.com/t/hosting-a-subdomain-on-webflow/59201)|[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/webflow-takeover.yaml)
Wix| Edge Case|[:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/231) || [:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/wix-takeover.yaml)
Wordpress|Yes| [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/pull/176)||[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/wordpress-takeover.yaml)
Worksites |Yes| [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/142) | |[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/main/http/takeovers/worksites-takeover.yaml)
WP Engine|No|||:x:
Zendesk|No| [:information_source:](https://github.com/EdOverflow/can-i-take-over-xyz/issues/23) | [:blue_book:](https://support.zendesk.com/hc/en-us/articles/203664356-Changing-the-address-of-your-Help-Center-subdomain-host-mapping-)|[:heavy_check_mark:](https://github.com/projectdiscovery/nuclei-templates/blob/076aa6cafde57ffd2e8781650525122f452e2338/http/takeovers/zendesk-takeover.yaml#L4)


# Stats 
| Total Takeovers | Active Takeovers | Inactive Takeovers | Edge Case Takeovers | 
   |------------------|-------------------|--------------------|---------------------| 
  | 89 | 51 | 21 | 17 | 
 
 | Takeovers with templates | Takeovers without templates| 
   |------------------|-------------------| 
  | 65 | 24 | 

