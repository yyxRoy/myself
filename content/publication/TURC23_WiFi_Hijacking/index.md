---
title: 'Traffic Hijacking in Wi-Fi Networks via ICMP Redirects'

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

date: '2023-07-29T00:00:00Z'
doi: ''

# Schedule page publish date (NOT publication's date).
publishDate: '2023-01-01T00:00:00Z'

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ['1']

# Publication name and optional abbreviated publication name.
publication: In [*Proceedings of the ACM Turing Award Celebration Conference - China 2023*](https://dl.acm.org/doi/10.1145/3603165.3607441), Wuhan China July 28 - 30, 2023
publication_short: In [*TURC 2023*](https://dl.acm.org/doi/10.1145/3603165.3607441), Wuhan China July 28 - 30, 2023

abstract: This paper uncovers a vulnerability involving identity spoofing through cross-layer interactions among Wi-Fi, IP, and ICMP protocols. The discovered vulnerability enables an off-path attacker to impersonate the Access Point (AP) of a Wi-Fi network, allowing the attacker to hijack plaintext traffic transmitted by wireless stations. We identify a design flaw in the Network Processing Units (NPUs) of widely-used chip manufacturers, which can be exploited by the attacker to spoof the AP and send ICMP redirect messages. By deceitfully mimicking a new AP within the network, the attacker successfully tricks other supplicants into believing that the attacker is a legitimate AP within the network. Consequently, the victim supplicants unknowingly forward their plaintext traffic to the attacker, leading to a successful Man-In-The-Middle (MITM) attack. Through extensive experimentation, we demonstrate that 55 popular AP routers and over 89% of real-world Wi-Fi networks are susceptible to the identified MITM attack.

# Summary. An optional shortened abstract.
summary: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellus ac convallis placerat. Proin tincidunt magna sed ex sollicitudin condimentum.

tags: []

# Display this page in the Featured widget?
featured: false

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://dl.acm.org/doi/pdf/10.1145/3603165.3607441'
url_code: ''
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: ''
url_source: ''
url_video: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
image:
  # caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/pLCdAaMFLTE)'
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
<!-- {{% callout note %}}
Click the _Cite_ button above to demo the feature to enable visitors to import publication metadata into their reference management software.
{{% /callout %}}

{{% callout note %}}
Create your slides in Markdown - click the _Slides_ button to check out the example.
{{% /callout %}}

Supplementary notes can be added here, including [code, math, and images](https://wowchemy.com/docs/writing-markdown-latex/). -->
