# Evaluation

A scientific paper consists of a constellation of artifacts that extend beyond the document itself: software, hardware, evaluation data and documentation, raw survey results, mechanized proofs, models, test suites, benchmarks, and so on. In some cases, the quality of these artifacts is as important as that of the document itself, yet many of our conferences offer no formal means to submit and evaluate anything but the paper itself. To address this shortcoming, we are running an optional artifact evaluation process, inspired by similar efforts in software engineering and other areas of science. USENIX Security will run for the first time an optional artifact evaluation process, inspired by similar efforts in software engineering and other areas of science.

## Artifact Submission Guidelines

### Step 1. Registration

By the registration deadline, please submit the abstract and PDF of your accepted USENIX Security '20 paper, as well as topics, conflicts, and any "optional bidding instructions" for potential reviewers via the [web submission form](https://sec20winterae.usenix.hotcrp.com/).

### Step 2. Package and Submit Artifact

By the artifact finalization deadline, please provide a stable URL or (if that is not possible) upload an archive of your artifact. You will no longer be able to change these after the artifact finalization deadline. For your artifact to be considered you also need to check the "ready for review" box before the finalization deadline.

We recommend creating a single web page at a stable URL that contains the artifact and instructions for installing and using the artifact (in case of software). For other types of artifacts, please make sure that they can be evaluated in a meaningful way, please describe your artifact in detail to simplify this process. If something is unclear, you will be contacted to clarify any questions regarding your artifact.

The artifact evaluation committee will read your accepted paper before evaluating the artifact. But it is quite likely that the artifact needs more documentation to use. In particular, please make concrete what claims you are making of the artifact, especially if these differ from the expectations set up by the paper. This is a place where you can tell us about difficulties we might encounter in using the artifact, or its maturity relative to the content of the paper. We are still going to evaluate the artifact relative to the paper, but this helps set expectations up front, especially in cases that might frustrate the reviewers without prior notice.

### Artifact Authors Are Not Anonymous

The artifact submissions are not anonymous. The reviewers will see the authors for each artifact from the start. So please do not waste your time trying to hide the artifact authors.

### Reviewer Anonymity

We ask that, during the evaluation period, you do not embed any analytics or other tracking in the website for the artifact or, if you cannot control this, that you do not access this data. This is important for maintaining the confidentiality of reviewers. If for some reason you cannot comply with this, please notify the chairs immediately such that we can discuss options.

### Packaging Artifacts

Authors should consider one of the following methods to package the software components of their artifacts (though the AEC is open to other reasonable formats as well):

-   **Source code:**If your artifact has very few dependencies and can be installed easily on several operating systems, you may submit source code and build scripts. However, if your artifact has a long list of dependencies, please use one of the other formats below.
-   **Virtual machine/container:** A virtual machine or Docker image containing the software application already set up with the right tool-chain and intended runtime environment. For example:

-   For raw data, the VM would contain the data and the scripts used to analyze it.
-   For a mobile phone application, the VM would have a phone emulator installed.
-   For mechanized proofs, the VM would have the right version of the theorem prover used.
-   We recommend using VirtualBox or Docker, since both are freely available on several platforms. An Amazon EC2 instance is also possible.

-   **Binary Installer:** Please indicate exactly which platform and other runtime dependencies your artifact requires.
-   **Live instance on the Web:** Ensure that it is available for the duration of the artifact evaluation process.
-   **Hardware:** In case your artifact requires special hardware (e.g., SGX or another type of trusted execution environment) or your artifact is actually a piece of hardware, please make sure that the reviewers can somehow access the device. Some kind of VPN access to the device might be an option, but due to anonymity we would need to discuss options—please contact the chairs in advance.
-   **Screencast:** A detailed screencast of the tool along with the results, especially if one of the following special cases applies:

-   The artifact needs proprietary/commercial software or proprietary data that is not easily available or cannot be distributed to the committee.
-   The artifact requires significant computation resources (e.g., more than 24 hours of execution time to produce the results) or requires huge data sets.
-   The artifact requires specific hard- or software that is not generally available in a typical lab and where no access can be provided in a reasonable way.

Remember that the Artifact Evaluation Committee (AEC) is attempting to determine whether the artifact meets the expectations set by the paper. If possible, package your artifact to help the committee easily evaluate this.

If you have any questions about how best to package your artifact, please do not hesitate to contact the AEC chairs, at

