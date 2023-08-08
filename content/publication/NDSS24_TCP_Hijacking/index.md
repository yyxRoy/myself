---
title: 'Exploiting Sequence Number Leakage: TCP Hijacking in NAT-Enabled Wi-Fi Networks'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - admin
  - Xuewei Feng
  - Qi Li
  - Kun Sun
  - Ziqiang Wang
  - Ke Xu


# Author notes (optional)
# author_notes:
  # - 'Equal contribution'
  # - 'Equal contribution'

date: '2023-08-15T00:00:00Z'
doi: ''

# Schedule page publish date (NOT publication's date).
publishDate: '2023-03-05T00:00:00Z'

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ['1']

# Publication name and optional abbreviated publication name.
publication: In [*Proceedings of the 31th Annual Network and Distributed System Security Symposium*](https://www.ndss-symposium.org/ndss2024/), San Diego, California, 27 February – 3 March, 2024, to appear
publication_short: In [*NDSS 2024*](https://www.ndss-symposium.org/ndss2024/), San Diego, California, 27 February – 3 March, 2024, to appear

abstract: 
  In this paper, we uncover a new side-channel vulnerability in the widely-used NAT port preservation strategy and an insufficient reverse path verification strategy of Wi-Fi routers, which allows an off-path attacker to infer if there is one victim client in the same network communicating with another host on the Internet using TCP. After detecting the presence of TCP connections between the victim client and the server, the attacker can evict the original NAT mapping and reconstruct a new mapping at the router by sending fake TCP packets due to the routers’ vulnerability of disabling TCP window tracking strategy, which has been faithfully implemented in most of the routers for years. In this way, the attacker can intercept TCP packets from the server and obtain the current sequence and acknowledgment numbers, which in turn allows the attacker to forcibly close the connection, poison the traffic in plain text, or reroute the server’s incoming packets to the attacker. 
 

  We test 67 widely used routers from 30 vendors and discover that 52 of them are affected by this attack. Also, we conduct an extensive measurement study on 93 real-world Wi-Fi networks. The experimental results show that 75 of these evaluated Wi-Fi networks (81%) are fully vulnerable to our attack. Our case study shows that it takes about 17.5, 19.4, and 54.5 seconds on average to terminate an SSH connection, download private files from FTP servers, and inject fake HTTP response packets with success rates of 87.4%, 82.6%, and 76.1%. We responsibly disclose the vulnerability and suggest mitigation strategies to all affected vendors and have received positive feedback, including acknowledgments, CVEs, rewards, and adoption of our suggestions.


# Summary. An optional shortened abstract.
summary: 

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
