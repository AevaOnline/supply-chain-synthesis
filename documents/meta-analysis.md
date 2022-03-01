Meta Analysis of the OSS Supply Chain Security Landscape
===

Background
---

This document focuses on the meta analysis -- that is, what are the social currents, tech trends, and externalities that affect all technical work in this domain, but which are not themselves technical in nature.

Externalities
---

The recent EO, and the timeline it imposes upon the NTIA, has drawn extraordinary attention to this problem domain and created an unusually ripe opportunity for media engagement and public outreach. A public request for comments from NTIA yielded responses from over 100 organizations and individuals around the world, and has created a fixed timeline against which many organizations are working under increased pressure.

Refs:
- [Executive Order on Improving the Nation's Cybersecurity | The White House](https://www.whitehouse.gov/briefing-room/presidential-actions/2021/05/12/executive-order-on-improving-the-nations-cybersecurity/) 
- [Workshop and Call for Position Papers on Standards and Guidelines to Enhance Software Supply Chain Security | NIST](https://www.nist.gov/itl/executive-order-improving-nations-cybersecurity/workshop-and-call-position-papers) 
- [Enhancing Software Supply Chain Security: Responses to Call for Position Papers on Standards and Guidelines | NIST](https://www.nist.gov/itl/executive-order-improving-nations-cybersecurity/enhancing-software-supply-chain-security) 

Meta Analysis
---

In the Minimum Elements For a Software Bill of Materials , published on 12 July, 2021, the NTIA has recommended a reasonably low bar, as a minimum should be, while also outlining areas where the industry is encouraged to go above and beyond this proposal.

As the industry collaborates to build SSCM solutions, we should all be mindful to remember that iterative improvement is improvement, and not to hold back any solution that is iteratively better than our current state of the art merely because it is not yet a perfect or complete solution.

If, on the other hand, the technical measures necessary to secure a global, distributed, open source software supply chain appear simple, it is only due to one’s distance from the technology. This is a fractal problem domain, with distinct challenges compared to the traditional enterprise domain. The closer one inspects any solution, the more the edges of the domain retreat from view. It is reminiscent of 

Evidence of this can be seen in the fragmentation of efforts across - and outside of - foundations, reflected in the breadth of responses to the NTIA’s call for positions, the diversity of projects enumerated below, and in the IETF discussions seeking to define a shared lexicon for this work.

Some SDL techniques common in closed-source development practices may not be applicable to open source projects, as the domains are sufficiently different. Several discussions on this topic have been had within the OpenSSF, particularly the Digital Identity Attestation WG.

Refs:

- [The Minimum Elements For a Software Bill of Materials (SBOM) | NTIA](https://www.ntia.doc.gov/files/ntia/publications/sbom_minimum_elements_report.pdf) 

Hardware Plays a Part
---

*TODO*

Trusting Trust
---

*TODO*

Refs:

- [Reflections on Trusting Trust](https://users.ece.cmu.edu/~ganger/712.fall02/papers/p761-thompson.pdf)
- [Countering "Trusting Trust"](https://www.schneier.com/blog/archives/2006/01/countering_trus.html)

Risks and Recommendations
---

The glamor of the press should not be conflated with sound engineering, but should not be dismissed. Well-run outreach work can generate a “snowball” effect, and transform small projects very rapidly, but must be sustained and well informed to have a lasting effect and yield healthy open source communities.

There is a risk in thinking this problem can be solved by borrowing a technical solution originally designed for a single corporate domain: implicit assumptions of workflow or business objectives may not be valid in other contexts.

There is also a risk in working to solve this through a standards-body: IETF processes take many years to bear fruit (a timeline incompatible with the EO), require a multi-stake-holder vetting process, and rely on real-world implementations as verification of the suitability of any specification.

Additionally, any solution which does not provide a native mechanism for interoperability among both providers and consumers of SBOM information will necessarily be subsumed in an abstraction layer, or fail to be widely adopted. Any hosted solution must also appear to prevent single-party control or influence, or other parties will not trust it and will invent and operate their own hosted solutions. These are realities of the requirements imposed by the EO, and reflect a change in the status quo as compared to one year ago. It is thus recommended to pay particular attention to format specifications, areas of extensibility, and operationalization requirements.

Given these seemingly-conflicting objectives and the risk of investing in efforts which may not materialize rapidly enough to satisfy the EO, tensions among participants in the projects are understandably high. 

A rational approach is, then, to work in parallel on implementations and on specifications, ensuring open channels of communication between those engaged in different efforts where possible and as often as possible.


