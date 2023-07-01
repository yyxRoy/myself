---
title: 'Man-in-the-Middle Attacks without Rogue AP: When WPAs Meet ICMP Redirects'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - Xuewei Feng
  - Qi Li
  - Kun Sun
  - admin
  - Ke Xu


# Author notes (optional)
# author_notes:
  # - 'Equal contribution'
  # - 'Equal contribution'

date: '2023-07-01T00:00:00Z'
doi: ''

# Schedule page publish date (NOT publication's date).
publishDate: '2023-01-01T00:00:00Z'

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ['1']

# Publication name and optional abbreviated publication name.
publication: In *IEEE Symposium on Security and Privacy 2023*
publication_short: In *S&P 2023*

abstract: Modern Wi-Fi networks are commonly protected by the security mechanisms, e.g., WPA, WPA2 or WPA3, and thus it is difficult for an attacker (amalicious supplicant) to hijack the traffic of other supplicants as a man-in-the-middle (MITM). In traditional Evil Twins attacks, attackers may deploy a bogus wireless access point (AP) to hijack the victim supplicants’ traffic (e.g., stealing credentials). In this paper, we uncover a new MITM attack that can evade the security mechanisms in Wi-Fi networks by spoofing the legitimate AP to send a forged ICMP redirect message to a victim supplicant and thus allow attackers to stealthily hijack the traffic from the victim supplicant without deploying any bogus AP. The core idea is to misuse the vulnerability of cross-layer interactions between WPAs and ICMP protocols, totally evading the link layer security mechanisms enforced by WPAs. We resolve two requirements to successfully launch our attack. First, when the attacker spoofs the legitimate AP to craft an ICMP redirect message, the legitimate AP cannot recognize and filter out those forged ICMP redirect messages. We uncover a new vulnerability (CVE-2022-25667) of the Network Processing Units (NPUs) in AP routers that restrict the AP routers from blocking fake ICMP error messages passing through the router. We test 55 popular wireless routers from 10 well-known AP vendors, and none of these routers can block the forged ICMP redirect messages due to this vulnerability. Second, we develop a new method to ensure the forged ICMP redirect message can evade the legitimacy check of the victim supplicant and then poison its routing table. We conduct an extensive measurement study on 122 real-world Wi-Fi networks, covering all prevalent Wi-Fi security modes. The experimental results show that 109 out of the 122 (89%) evaluated Wi-Fi networks are vulnerable to our attack. Besides notifying the vulnerability to the NPU manufacturers and the AP vendors, we develop two countermeasures to throttle the identified attack.

# Summary. An optional shortened abstract.
summary: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellus ac convallis placerat. Proin tincidunt magna sed ex sollicitudin condimentum.

tags: []

# Display this page in the Featured widget?
featured: false

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: ''
url_code: ''
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: ''
url_source: ''
url_video: 'https://www.youtube.com/watch?v=1GFg_h0OyWs&list=PL0pRF4xvoD0kRsa5AeL9ncGw7CnLdIr7A&index=104&t=777s&ab_channel=IEEESymposiumonSecurityandPrivacy'

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
image:
  caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/pLCdAaMFLTE)'
  focal_point: ''
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
# projects:
  # - example

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
# slides: example
---

{{% callout note %}}
Click the _Cite_ button above to demo the feature to enable visitors to import publication metadata into their reference management software.
{{% /callout %}}

{{% callout note %}}
Create your slides in Markdown - click the _Slides_ button to check out the example.
{{% /callout %}}

Supplementary notes can be added here, including [code, math, and images](https://wowchemy.com/docs/writing-markdown-latex/).
