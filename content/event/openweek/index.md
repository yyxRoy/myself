---
title: Open Week of CS Student Achievements

event: Open Week of CS Student Achievements
event_url: https://sp2023.ieee-security.org/

location: Tsinghua University, Beijing, China
# address:
#   street: 450 Serra Mall
#   city: Stanford
#   region: CA
#   postcode: '94305'
#   country: United States

summary: In the 2023 Open Week of CS Student Achievements, I presented our paper "Exploiting Sequence Number Leakage - TCP Hijacking in NAT-Enabled Wi-Fi Networks"

abstract: 'In this paper, we uncover a new side-channel vulnerability in the widely-used NAT port preservation strategy and an insufficient reverse path verification strategy of Wi-Fi routers, which allows an off-path attacker to infer if there is one victim client in the same network communicating with another host on the Internet using TCP. After detecting the presence of TCP connections between the victim client and the server, the attacker can evict the original NAT mapping and reconstruct a new mapping at the router by sending fake TCP packets due to the routers’ vulnerability of disabling TCP window tracking strategy, which has been faithfully implemented in most of the routers for years. In this way, the attacker can intercept TCP packets from the server and obtain the current sequence and acknowledgment numbers, which in turn allows the attacker to forcibly close the connection, poison the traffic in plain text, or reroute the server’s incoming packets to the attacker.
We test 67 widely used routers from 30 vendors and discover that 52 of them are affected by this attack. Also, we conduct an extensive measurement study on 93 real-world Wi-Fi networks. The experimental results show that 75 of these evaluated Wi-Fi networks (81%) are fully vulnerable to our attack. Our case study shows that it takes about 17.5, 19.4, and 54.5 seconds on average to terminate an SSH connection, download private files from FTP servers, and inject fake HTTP response packets with success rates of 87.4%, 82.6%, and 76.1%. We responsibly disclose the vulnerability and suggest mitigation strategies to all affected vendors and have received positive feedback, including acknowledgments, CVEs, rewards, and adoption of our suggestions.'

# Talk start and end times.
#   End time can optionally be hidden by prefixing the line with `#`.
date: '2023-09-14T13:00:00Z'
date_end: '2023-09-14T15:00:00Z'
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
url_video: ''

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
