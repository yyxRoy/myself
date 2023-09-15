---
title: S&P 2023

event: S&P 2023 Conference
event_url: https://sp2023.ieee-security.org/

location: San Francisco, CA at the Hyatt Regency & Online
# address:
#   street: 450 Serra Mall
#   city: Stanford
#   region: CA
#   postcode: '94305'
#   country: United States

summary: In the 2023 44th IEEE Symposium on Security and Privacy, I presented our paper "Man-in-the-Middle Attacks without Rogue AP - When WPAs Meet ICMP Redirects"

abstract: 'Modern Wi-Fi networks are commonly protected by the security mechanisms, e.g., WPA, WPA2 or WPA3, and thus it is difficult for an attacker (a malicious supplicant) to hijack the traffic of other supplicants as a man-in-the-middle (MITM). In traditional Evil Twins attacks, attackers may deploy a bogus wireless access point (AP) to hijack the victim supplicants’ traffic (e.g., stealing credentials). In this paper, we uncover a new MITM attack that can evade the security mechanisms in Wi-Fi networks by spoofing the legitimate AP to send a forged ICMP redirect message to a victim supplicant and thus allow attackers to stealthily hijack the traffic from the victim supplicant without deploying any bogus AP. The core idea is to misuse the vulnerability of cross-layer interactions between WPAs and ICMP protocols, totally evading the link layer security mechanisms enforced by WPAs. We resolve two requirements to successfully launch our attack. First, when the attacker spoofs the legitimate AP to craft an ICMP redirect message, the legitimate AP cannot recognize and filter out those forged ICMP redirect messages. We uncover a new vulnerability (CVE-2022-25667) of the Network Processing Units (NPUs) in AP routers that restrict the AP routers from blocking fake ICMP error messages passing through the router. We test 55 popular wireless routers from 10 well-known AP vendors, and none of these routers can block the forged ICMP redirect messages due to this vulnerability. Second, we develop a new method to ensure the forged ICMP redirect message can evade the legitimacy check of the victim supplicant and then poison its routing table. We conduct an extensive measurement study on 122 real-world Wi-Fi networks, covering all prevalent Wi-Fi security modes. The experimental results show that 109 out of the 122 (89%) evaluated Wi-Fi networks are vulnerable to our attack. Besides notifying the vulnerability to the NPU manufacturers and the AP vendors, we develop two countermeasures to throttle the identified attack.'

# Talk start and end times.
#   End time can optionally be hidden by prefixing the line with `#`.
date: '2023-05-23T13:00:00Z'
date_end: '2023-05-26T15:00:00Z'
all_day: false

# Schedule page publish date (NOT talk date).
publishDate: '2023-01-01T00:00:00Z'

authors: []
tags: []

# Is this a featured talk? (true/false)
featured: false

image:
  # caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/bzdhc5b3Bxs)'
  focal_point: Right

# links:
  # - icon: twitter
  #   icon_pack: fab
  #   name: Follow
  #   url: https://twitter.com/georgecushen
url_code: ''
url_pdf: ''
url_slides: ''
url_video: 'https://www.youtube.com/watch?v=1GFg_h0OyWs&list=PL0pRF4xvoD0kRsa5AeL9ncGw7CnLdIr7A&index=104&t=777s&ab_channel=IEEESymposiumonSecurityandPrivacy'

# Markdown Slides (optional).
#   Associate this talk with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: example

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
# projects:
#   - example
---

<!-- {{% callout note %}}
Click on the **Slides** button above to view the built-in slides feature.
{{% /callout %}}

Slides can be added in a few ways:

- **Create** slides using Wowchemy's [_Slides_](https://wowchemy.com/docs/managing-content/#create-slides) feature and link using `slides` parameter in the front matter of the talk file
- **Upload** an existing slide deck to `static/` and link using `url_slides` parameter in the front matter of the talk file
- **Embed** your slides (e.g. Google Slides) or presentation video on this page using [shortcodes](https://wowchemy.com/docs/writing-markdown-latex/).

Further event details, including [page elements](https://wowchemy.com/docs/writing-markdown-latex/) such as image galleries, can be added to the body of this page. -->
