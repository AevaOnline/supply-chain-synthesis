N.B. Everyone is welcome to add missing projects. If you're uncertain how to categorize it, please add at the end of this section. If you have concerns about an existing categorization (i.e., think a project belongs in a different category) please add a comment.

If you are a project owner, please provide a concise description of the project scope; if not, you may still add a description, and please add a comment indicating that it needs to be verified. When in doubt, copy a sentence or two from the project's home page.

-   Formats, Specifications, and Standards
    -   [SPDX](https://spdx.dev/specifications/)
    -   [CycloneDX](https://github.com/CycloneDX/)
    -   [SWID](https://standards.iso.org/iso-iec/19770/-2/2015-current/schema.xsd) ([CoSWID](https://www.ietf.org/archive/id/draft-ietf-sacm-coswid-18.html), [NISTIR 8060](https://doi.org/10.6028/NIST.IR.8060))
    -   CPE, SHI, SParts,
    -   [OWASP SCVS](https://owasp.org/www-project-software-component-verification-standard/): standard that provides controls and best practices for increasing trust in your dependencies in your supply chain.
    -   [package-url/purl-spec:](https://github.com/package-url/purl-spec) A minimal specification for purl aka. a package "mostly universal" URL, join the discussion at https://gitter.im/package-url/Lobby (github.com)
-   SBOM generation & distribution tools
    -   [Syft](https://github.com/anchore/syft): CLI tool and library for generating a Software Bill of Materials from container images and filesystems
    -   [Tern](https://github.com/tern-tools/tern): Software composition analysis tool and Python library that generates a Software Bill of Materials for container images and Dockerfiles. The SBoM that Tern generates will give you a layer-by-layer view of what's inside your container in a variety of formats including human-readable, JSON, HTML, SPDX and more. 
    -   [in-toto](https://in-toto.io/): provides a framework to protect the integrity of the software supply chain. It does so by verifying that each task in the chain is carried out as planned, by authorized personnel only, and that the product is not tampered with in transit.
    -   [ORAS Artifacts](https://github.com/oras-project/artifacts-spec/): provides storing any file based content as a reference to existing artifact content stored in OCI Registry. Examples: Notary v2 signatures, SBoMs, Security Scanner Results, GPL Source
    -   [The Update Framework (TUF)](https://theupdateframework.io/): a compromise resilient framework for secure distribution and updating of artifacts and artifact metadata.
    -   [Notary v2](https://github.com/notaryproject/notaryproject#notary-v2-overview): provides for multiple signatures of an [OCI Artifact](https://github.com/opencontainers/artifacts) (including container images) to be persisted in an [OCI conformant](https://github.com/opencontainers/oci-conformance) registry. Artifacts are signed (nv2 sign) with private keys, and validated with public keys (nv2 verify). [ Status report from the project indicates work still in progress, ETA Fall '21\. ]
    -   [K8sbom](https://github.com/kubernetes/release/blob/master/docs/bom/create-a-bill-of-materials.md) - a set of libraries to produce fully compliant SPDX SBOMs. These tools support license scanning, image layer analyzers, processing of golang dependencies, and other features. 
    -   [SPDX SBoM CLI generator](https://github.com/spdx/spdx-sbom-generator) - a tool to help those in the community that want to generate SPDX Software Bill of Materials (SBOMs) with current package managers. It has a command line Interface (CLI) that lets you generate SBOM information, including components, licenses, copyrights, and security references of your software using SPDX v2.2 specification and aligning with the current known minimum elements from NTIA. It automatically determines which package managers or build systems are actually being used by the software.  Supports: GoMod (go), Cargo (Rust), Composer (PHP), DotNet (.NET), Maven (Java), NPM (Node.js), Yarn (Node.js), PIP (Python), Pipenv (Python), Gems (Ruby), Swift Package Manager (Swift)
    -   [Sigstore](https://sigstore.dev/what_is_sigstore/): empowers software developers to securely sign software artifacts such as release files, container images, binaries, bill of material manifests and more. Signing materials are then stored in a tamper-resistant public log.
        -   Comprised of several projects: sigstore, rekor, cosign, fulcio, ...
-   Scanning and analysis tools
    -   [Grype](https://github.com/anchore/grype): A vulnerability scanner for container images and filesystems.
    -   [oss-review-toolkit/ort](https://github.com/oss-review-toolkit/ort): A suite of tools to assist with reviewing Open Source Software dependencies.
    -   [Repology (github.com)](https://github.com/repology) and [Libraries.io (github.com)](https://github.com/librariesio)
    -   [nexB/scancode-toolkit:](https://github.com/nexB/scancode-toolkit) ScanCode detects licenses, copyrights, package manifests & dependencies and more by scanning code ... to discover and inventory open source and third-party packages used in your code.
    -   [recipy/recipy:](https://github.com/recipy/recipy)  Effortless method to record provenance in Python 
    -   [DependencyTrack/dependency-track:](https://github.com/DependencyTrack/dependency-track)  Dependency-Track is an intelligent Component Analysis platform that allows organizations to identify and reduce risk in the software supply chain. 
    -   [tern-tools/tern](https://github.com/tern-tools/tern): Tern is a software composition analysis tool and Python library that generates a Software Bill of Materials for container images and Dockerfiles. The SBoM that Tern generates will give you a layer-by-layer view of what's inside your container in a variety of formats including human-readable, JSON, HTML, SPDX and more.
    -   [ComponentDetection](https://github.com/microsoft/component-detection): ComponentDetection is a package scanning tool intended to be used at build time. CD produces a graph-based output of all detected components and supports a variety of open source package ecosystems.
-   Policy & admission control tools
    -   [Tekton Chains](https://github.com/tektoncd/chains): a Kubernetes Custom Resource Definition (CRD) controller that allows you to manage your supply chain security in Tekton.
    -   [Connaisseur](https://sse-secure-systems.github.io/connaisseur/v2.0.0/): A Kubernetes admission controller to integrate container image signature verification and trust pinning into a cluster.
    -   [Open Policy Agent](https://www.openpolicyagent.org/): policy-based admission control for cloud native systems.
-   Identity systems
    -   [SPIFFE/Spire](https://github.com/spiffe/spire): a toolchain of APIs for establishing trust between software systems across a wide variety of hosting platforms
    -   [PARSEC](https://github.com/parallaxsecond/parsec): an open-source initiative to provide a common API to hardware security and cryptographic services in a platform-agnostic way. This abstraction layer keeps workloads decoupled from physical platform details, enabling cloud-native delivery flows within the data center and at the edge
    -   [Keylime](https://github.com/keylime/keylime): provides an end-to-end solution for bootstrapping hardware rooted cryptographic trust for remote machines, the provisioning of encrypted payloads, and run-time system integrity monitoring
    -   [Veraison](https://github.com/veraison/veraison): will build software components that can be used to build Attestation Verification Services
        -   (Aeva's opinion) An early project release from Arm, which appears to be promising but may not be functionally complete yet.
    -   [CHARRA](https://github.com/Fraunhofer-SIT/charra): PoC to establish underlying trust relationships with an Attester using TPMs. Build for constrained node environments and application in firmware.
-   Miscellaneous // not yet categorised [ PLEASE ADD HERE ]
    1.  [SLSA](https://github.com/slsa-framework/slsa): security framework from source to service, giving anyone working with software a common language for increasing levels of software security and supply chain integrity.
    2.  [Trillian](https://github.com/google/trillian): A transparent, highly scalable and cryptographically verifiable data store. 
    3.  <https://github.com/CycloneDX/cyclonedx-cli>
    4.  <https://github.com/vmware-samples/containers-with-sboms>: End to End SBOM generation, signing, and distribution for container images

Work streams not yet in a project // which don't yet have code
--------------------------------------------------------------

-   [SCIM](https://github.com/microsoft/scim): supports the ongoing verification of artifacts, including hardware and software components, where the authenticity of entities, evidence, policy, and artifacts can be assured and the actions of entities can be guaranteed to be trustworthy, authorized, non-repudiable, immutable, and auditable. 
-   [GitBOM](https://hackmd.io/@aeva/draft-gitbom-spec): a novel and minimalistic approach to generating artifact trees at build time, thereby enabling launch-time comparison of vulnerability data against a complete artifact tree for open source projects.
-   (NTIA) [Vulnerability Exploitability eXchange](https://docs.google.com/document/d/1sylBGNooKtf220RHQn1I8pZRmqXZQADDQ_TOABrKTpA/edit#heading=h.ss425olznxo) draft
-   (Google) [Shared Vulnerability Format](https://docs.google.com/document/d/1sylBGNooKtf220RHQn1I8pZRmqXZQADDQ_TOABrKTpA/edit#heading=h.ss425olznxo) proposal