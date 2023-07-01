---
title: "A Method for Enhancing Network Security of the Transport Layer by Leveraging the Lightweight Chain Verification"
authors:
- Xuewei Feng
- Ke Xu
- Qi Li
- admin
- Min Zhu
- Songtao Fu 
# author_notes:
# - "Equal contribution"
# - "Equal contribution"
date: "2023-03-29T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2023-03-29T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: "*Journal of Software"
publication_short: ""

abstract: The transport layer is a key component in network protocol stack, which is responsible for providing end-to-end services for applications between different end hosts on the Internet. Existing transport layer protocols such as TCP provide users with some basic protections, e.g., error controls and acknowledgements, which ensures the consistency of user datagram to a certain extent. However, these basic protections are not adequate to defend various attacks on the Internet. For example, the sequence number of TCP segments is easy to be guessed and inferred, and the calculation of the datagram’s checksum depends on the vulnerable one's complement sum. As a result, the existing transport layer security mechanisms cannot guarantee the integrity and security of the datagram transferred on the Internet, which allows a remote attacker to craft a fake datagram and inject it into the target network stream, thus poisoning the target network stream. The attack against the transport layer occurs at the basic layers of the network protocol stack, which can bypass the security mechanisms enforced at the upper application layer (e.g., user name and password) and thus cause serious damages to the network infrastructure. In this paper, after investigating various prior attacks over network protocols and the related security vulnerabilities, we propose a security mechanism LightCTL based on the lightweight chain verification, which can be deployed at the transport layer to guarantee the integrity of the datagram transferred on the Internet. Based on the hash verification, LightCTL enables both peers of a TCP connection to create a verifiable consensus on transport layer datagrams, so as to prevent attackers from stealing and forging sensitive information. As a result, LightCTL can successfully foil various attacks against network protocol stack, including TCP connection reset attacks based on sequence number inferring, TCP hijacking attacks, SYN flooding attacks, Man-in-The-Middle attacks, replay attacks. Besides, LightCTL does not need to modify the protocol stack of intermediate network devices such as routers. It only needs to modify the checksum and the related parts of the end hosts’ protocol stack. Therefore, LightCTL is easy to be deployed in the real world and significantly improves the security of networks.

# Summary. An optional shortened abstract.
# summary: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellus ac convallis placerat. Proin tincidunt magna sed ex sollicitudin condimentum.

tags:
- Source Themes
featured: false

# links:
# - name: ""
#   url: ""
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
  # caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/jdD8gXaTZsc)'
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects: []

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
# slides: example
---

<!-- {{% callout note %}}
Click the *Cite* button above to demo the feature to enable visitors to import publication metadata into their reference management software.
{{% /callout %}} -->

<!-- {{% callout note %}}
Create your slides in Markdown - click the *Slides* button to check out the example.
{{% /callout %}} -->

<!-- Supplementary notes can be added here, including [code, math, and images](https://wowchemy.com/docs/writing-markdown-latex/). -->
