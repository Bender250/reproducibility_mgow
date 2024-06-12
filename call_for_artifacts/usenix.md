# Evaluation

A scientific paper consists of a constellation of artifacts that extend beyond the document itself: software, hardware, evaluation data and documentation, raw survey results, mechanized proofs, models, test suites, benchmarks, and so on. In some cases, the quality of these artifacts is as important as that of the document itself, yet many of our conferences offer no formal means to submit and evaluate anything but the paper itself. To address this shortcoming, USENIX Security will run an optional artifact evaluation process, inspired by similar efforts in software engineering and other areas of science.


## Artifact Evaluation Information

### Overview

A scientific paper consists of a constellation of artifacts that extend beyond the document itself: software, hardware, evaluation data and documentation, raw survey results, mechanized proofs, models, test suites, benchmarks, and so on. In some cases, the quality of these artifacts is as important as that of the document itself. To emphasize the importance of such artifacts, the benefits to the authors and the community as a whole, and promote the reproducibility of experimental results, USENIX Security will run its fourth (optional) AE this year. The AEC will review each submitted artifact and also grant Distinguished Artifact Awards to outstanding artifacts accepted to USENIX Security '23.

### Process

To maintain a wall of separation between paper review and the artifacts, authors will be given the option to submit their artifacts only _after_ their papers have been accepted for publication at USENIX Security. The artifact submission deadline is around five weeks after the paper notification date, but a first stub submission to register the artifact is required around two weeks after the paper notification date. By the artifact submission deadline, authors can submit their artifacts, [Artifact Appendix](https://secartifacts.github.io/usenixsec2023/appendix/usesec23-ae-latex.zip), and other supporting information of their accepted USENIX Security 2023 paper [via the submission form](https://sec23winterae.usenix.hotcrp.com/) using the provided [submission instructions](https://secartifacts.github.io/usenixsec2023/instructions).

At artifact submission time, authors can provide artifacts including software, hardware, data sets, survey results, test suites, mechanized (but not paper) proofs, access to special hardware, and so on. In addition, authors can request their artifact to be evaluated towards one, two, or all three of the following badges: [Artifacts Available](https://secartifacts.github.io/usenixsec2023/badges), [Artifacts Functional](https://secartifacts.github.io/usenixsec2023/badges), and

### Badges

Submitted artifacts could select to be evaluated against the following badges:

**Artifacts Available:** To earn this badge, the AEC must judge that the artifacts associated with the paper have been made available for retrieval, permanently and publicly. The archived copy of the artifacts must be accessible via a stable reference or DOI. For this purpose, we recommend Zenodo, but other valid hosting options include institutional and third-party digital repositories (e.g., [Zenodo](https://zenodo.org/), [FigShare](https://figshare.com/), [Dryad](https://datadryad.org/stash/), [Software Heritage](https://archive.softwareheritage.org/), [GitHub](https://github.com/), or [GitLab](https://about.gitlab.com/) — **not** personal webpages). For repositories that can evolve over time (e.g., GitHub), a stable reference to the evaluated version (e.g., a URL pointing to a commit hash or tag) rather than the evolving version reference (e.g., a URL pointing to a mere repository) is required. Note that the stable reference provided at submission time is for the purpose of Artifact Evaluation. Since the artifact can potentially evolve during the evaluation to address feedback from the reviewers, another (potentially different) stable reference will be later collected for the final version of the artifact. Other than making the artifacts available, this badge does not mandate any further requirements on functionality, correctness, or documentation.

**Artifacts Functional:** To earn this badge, the AEC must judge that the artifacts conform to the expectations set by the paper in terms of functionality, usability, and relevance. In short, do the artifacts work and are they useful for producing outcomes associated with the paper? The AEC will consider three aspects of the artifacts in particular.  
**Documentation**: are the artifacts sufficiently documented to enable them to be exercised by readers of the paper?  
**Completeness**: do the submitted artifacts include all of the key components described in the paper?  
**Exercisability**: do the submitted artifacts include the scripts and data needed to run the experiments described in the paper, and can the software be successfully executed?

**Results Reproduced:** To earn this badge, the AEC must judge that they can use the submitted artifacts to obtain the main results presented in the paper. In short, is it possible for the AEC to independently repeat the experiments and obtain results that support the main claims made by the paper? The goal of this effort is not to reproduce the results exactly, but instead to generate results independently within an allowed tolerance such that the main claims of the paper are validated.
# Submission instructions

Artifacts must be packaged to ease evaluation and include an [artifact appendix](https://secartifacts.github.io/usenixsec2023/instructions#artifact-appendix). Packaging is not only about evaluation but about future use of the artifact by other researchers who may want to build on top of it or use it as a baseline. In addition, consider how you plan to distribute your artifact.

Please see our [tips](https://secartifacts.github.io/usenixsec2023/tips) page for insights on how to build great research artifacts.

Finally submit your artifact and its appendix via HotCRP to:

-   [Summer](https://sec23summerae.usenix.hotcrp.com/)
-   [Fall](https://sec23fallae.usenix.hotcrp.com/)
-   [Winter](https://sec23winterae.usenix.hotcrp.com/)

If you have any questions about how best to package your artifact, contact the AEC chairs.

_Destructive Artifacts_: Some artifacts may attempt to perform malicious or destructive operations by design. These cases should be boldly and explicitly flagged in detail at artifact submission time so the AEC can take appropriate precautions before installing and running these artifacts. Please contact the AEC chairs if you believe that your artifacts fall into this category.

_Camera-Ready Submission Instructions_: After an artifact evaluation concluded, we will collect a camera-ready version of all artifacts receiving at least one badge. This includes information about the artifact location, the appendix, and similar supplemental material. The instructions will be shared via eMail when the badge decisions are announced.

## Packaging[Permalink](https://secartifacts.github.io/usenixsec2023/instructions#packaging "Permalink")

Your artifact package must include an obvious “read me” document containing suitable instructions and documentation. A tool without a quick tutorial is generally very difficult to use. Similarly, a dataset is useless without some explanation on how to browse the data. Please see the [badges](https://secartifacts.github.io/usenixsec2023/badges) page for more details on what the instructions should contain.

Authors should consider one of the following methods to package the software components of their artifacts (although the AEC is open to other reasonable formats as well):

-   _Source code:_ If your artifact has few dependencies and can be installed easily on several operating systems, you may submit source code and build scripts. However, if your artifact has a long list of dependencies, please use one of the other formats below.
    
-   _Container/virtual machine:_ We recommend using a format that is easy for evaluators to work with, such as Docker images. In any case, the Dockerfile or script used to initialize the virtual machine should be available. Consider preparing the right toolchain and runtime environment.
    
-   _Live instance on the web:_ Ensure that it is available during the artifact evaluation process.
    
-   _Internet-accessible hardware:_ If your artifact requires special hardware (e.g., SGX or another trusted execution environment), or if your artifact is actually a piece of hardware, please make sure that evaluators can access the device. VPN/SSH-based access to the device might be an option (in that case, please provide the SSH private access key directly in your submission to reduce time to gain access to hardware).
    

## Artifact Storage[Permalink](https://secartifacts.github.io/usenixsec2023/instructions#artifact-storage "Permalink")

Great artifacts are easy to find and stored for a long time. The archived copy of the artifacts (necessary to qualify for the Artifacts Available badge) must be accessible via a stable reference or DOI. For this purpose, we recommend Zenodo, but other valid hosting options include institutional and third-party digital repositories (e.g., [Zenodo](https://zenodo.org/), [FigShare](https://figshare.com/), [Dryad](https://datadryad.org/stash/), [Software Heritage](https://archive.softwareheritage.org/), [GitHub](https://github.com/), or [GitLab](https://about.gitlab.com/). For repositories that can evolve over time (e.g., GitHub), a stable reference to the evaluated version (e.g., a URL pointing to a commit hash or tag) rather than the evolving version reference (e.g., a URL pointing to a mere repository) is required. Note that the stable reference provided at submission time is for the purpose of Artifact Evaluation. Since the artifact can potentially evolve during the evaluation to address feedback from the reviewers, another (potentially different) stable reference will be later collected for the final version of the artifact.

## Artifact Appendix[Permalink](https://secartifacts.github.io/usenixsec2023/instructions#artifact-appendix "Permalink")

The artifact appendix is a self-contained document which describes a roadmap for evaluators. This includes a description of the hardware, software, and configuration requirements, as well as the major claims made by the paper and how to reproduce each claim through your artifact. Linking the claims of the paper to the artifact is a necessary step that ultimately allows artifact evaluators to reproduce your results. It is of foremost importance that you state your paper’s key results and claims clearly. This is especially important if you think that these claims differ from the expectations set up by your paper. If possible, the appendix should also describe how to compare the results of a reproduced experiment to the ones found in the paper (e.g., by providing access to the underlying dataset of the results).

The intention for the artifact appendix is to be published in conjunction with your artifact. A template for the artifact appendix can be found here: [LaTeX Template](https://secartifacts.github.io/usenixsec2023/appendix/usesec23-ae-latex.zip) and [PDF Example](https://secartifacts.github.io/usenixsec2023/appendix/usesec23-appendix.pdf).

**Artifact Appendices are recommended to be 3 pages max.**

### usenixbadges.sty — affix USENIX Artifact Evaluation badges[Permalink](https://secartifacts.github.io/usenixsec2023/instructions#usenixbadgessty--affix-usenix-artifact-evaluation-badges "Permalink")

The `usenixbadges` LaTeX style file affixes USENIX Artifact Evaluation badges to the front page of a USENIX-formatted paper (or standalone Appendix). You must use it to add badges to your final (camera-ready) artifact appendix. You may also want to use it to add the badges to a self-hosted USENIX Security paper as well (which we recommend having the artifact appendix appended at the end). Download the [usenixbadges](https://secartifacts.github.io/usenixsec2023/appendix/usenix23-badges.zip) package and follow the instructions below.

#### INSTALLATION[Permalink](https://secartifacts.github.io/usenixsec2023/instructions#installation "Permalink")

Put `usenixbadges.sty` and the `usenixbadges-*.pdf` graphics files in the directory that contains the LaTeX source for your paper. (Really, you can put them anywhere in LaTeX’s search path, but the simplest thing is to put the files in the same directory as your paper’s LaTeX source files.)

#### USAGE[Permalink](https://secartifacts.github.io/usenixsec2023/instructions#usage "Permalink")

In the preamble of your LaTeX document, insert a line like this:

```
  \usepackage[<options>]{usenixbadges}
```

In the options, list the badges that have been awarded to your paper. The possible badges are:

-   `available` — affix the “Artifacts Available” badge
-   `functional` — affix the “Artifacts Functional” badge
-   `reproduced` — affix the “Results Reproduced” badge

Example:

```
  %% Affix the indicated badges to the paper.
  \usepackage[available,functional]{usenixbadges}
```

Tips:

In your LaTeX document, the `\usepackage[...]{usenixbadges}` directive must come after `\documentclass` and before `\begin{document}`.

If your LaTeX document has many `\usepackage` directives, put `\usepackage[...]{usenixbadges}` near the end of those. This may avoid problems relating to conflicting options for the `graphicx` package.

### Artifact Evaluation Committee Membership

The AEC will consist of about 30-40 members. We intend the AEC members to be a combination of senior graduate students, postdocs, and researchers, identified with the help of the USENIX Security Program Committee.

Qualified graduate students are often in a much better position than many researchers to handle the diversity of systems expectations we will encounter. In addition, these graduate students represent the future of the community, so involving them in this process early will help push this process forward. We are convinced that participation in the AEC can provide useful insight into both the value of artifacts, the process of artifact evaluation, and help establish community norms for artifacts. We therefore seek to include a broad cross-section of the USENIX Security community on the AEC.

Naturally, the AEC chairs will devote considerable attention to both mentoring and monitoring the junior members of the AEC, helping to educate the students on their power and responsibilities.

The AEC chairs will also grant Distinguished Artifact Reviewer Awards to AEC members who have contributed with outstanding efforts during the Artifact Evaluation and constructive feedback to authors.

If you are interested in becoming a part of the AEC, please complete [this online form](https://docs.google.com/forms/d/e/1FAIpQLSe3XfSZ4bVxJCp0IcywjUzfNCbPeogRg_gROYYu8xQZw8oYOg/viewform). Deadline: Saturday, September 25, 2021. You can reach us at [sec22aec@usenix.org](mailto:sec22aec@usenix.org) with any questions.

## Artifact Submission Guidelines

### Packaging and Submitting the Artifact

By the artifact registration deadline, please submit the abstract and PDF of your accepted USENIX Security 2022 paper (as well as topics and conflicts) via the [submission form](https://sec22winterae.usenix.hotcrp.com/).

Additionally, please provide instructions on how to access a working copy of your artifact for the purpose of Artifact Evaluation. For instance, this may involve providing a URL to a repository/archive of your artifact or instructions to get remote (e.g., SSH) access to a special evaluation platform. Note that the artifact does not need to be anonymized and you may update the working copy of your artifact during the Artifact Evaluation (in response to comments from the reviewers in the author discussion phase). For your artifact to be considered, you also need to check the "ready for review" box before the finalization deadline.

If you are applying for an Artifact Functional and/or Results Reproduced badge, the artifact should include a README file that gives detailed instructions on how to get it working, how to run your experiments, and how to satisfy all the relevant hardware/software requirements. If something is unclear, you will be contacted to clarify any questions regarding your artifact. Feel free to reach out in advance in case you have any questions.

The artifact evaluation committee will read your accepted paper before evaluating the artifact. Authors should also submit the unified [Artifact Appendix](https://www.usenix.org/sites/default/files/conference-files/sec22_ae_appendix_template_v20220119.zip) using the following [guidelines](https://www.usenix.org/conference/usenixsecurity22/artifact-appendix-guidelines). In particular, please make concrete what claims you are making of the artifact, especially if these differ from the expectations set up by the paper. This is a place where you can tell us about difficulties we might encounter in using the artifact, or its maturity relative to the content of the paper. We are still going to evaluate the artifact relative to the paper, but this helps set expectations upfront, especially in cases that might frustrate the reviewers without prior notice.

Note that, if you are awarded any badges, we will later collect the final version of your Artifact Appendix to be published on the USENIX website and in the next edition's proceedings. To prepare the final version, please follow the appropriate [instructions](https://www.usenix.org/conference/usenixsecurity22/final-artifact-appendix-instructions).

### Artifact Authors Not Anonymous

The artifact submissions are not anonymous. The reviewers will see the authors for each artifact from the start. Please do not waste your time trying to hide the artifact authors.

### Reviewer Anonymity

We ask that, during the evaluation period, you do not embed any analytics or other tracking in the Web site for the artifact or, if you cannot control this, that you do not access this data. This is important for maintaining the confidentiality of reviewers. If for some reason you cannot comply with this, please notify the chairs immediately such that we can discuss options.

### Packaging Artifacts

Authors should consider one of the following methods to package the software components of their artifacts (though the AEC is open to other reasonable formats as well):

-   **Source code:** If your artifact has very few dependencies and can be installed easily on several operating systems, you may submit source code and build scripts. However, if your artifact has a long list of dependencies, please use one of the other formats below.
-   **Virtual machine/container:** A virtual machine or Docker image containing software application already setup with the right tool-chain and intended runtime environment. For example:

-   For raw data, the VM would contain the data and the scripts used to analyze it.
-   For a mobile phone application, the VM would have a phone emulator installed.
-   For mechanized proofs, the VM would have the right version of the theorem prover used.

-   **We recommend using VirtualBox or Docker:** Both are freely available on several platforms. An Amazon EC2 instance is also possible.
-   **Binary Installer:** Please indicate exactly which platform and other runtime dependencies your artifact requires.
-   **Live instance on the Web:** Ensure that it is available for the duration of the artifact evaluation process.
-   **Remote machine:** In case your artifact requires special hardware (e.g., SGX or another type of trusted execution environment), your artifact is actually a piece of hardware, or uses confidential/proprietary/licensed software, please make sure that the reviewers can somehow access a target evaluation machine. Some kind of VPN/SSH access to the device might be an option, but please preserve reviewers’ anonymity, e.g., by explicitly asking reviewers a public key and disabling IP address or geolocation logging.

Remember that the AEC is attempting to determine whether the artifact meets the expectations set by the paper. If possible, package your artifact to help the committee easily evaluate this. This can for example be achieved via automated test cases that reproduce the experiments described in the paper or a step-by-step documentation to help setting up the artifact.

If you have any questions about how best to package your artifact, please do not hesitate to contact the AEC chairs, at [sec22aec@usenix.org](mailto:sec22aec@usenix.org).

### Further Advice

There are several sources of good advice about preparing artifacts for evaluation. These three are particularly noteworthy:

-   [HOWTO for AEC Submitters](https://docs.google.com/document/d/1pqzPtLVIvwLwJsZwCb2r7yzWMaifudHe1Xvn42T4CcA/edit), by Dan Barowy, Charlie Curtsinger, Emma Tosch, John Vilk, and Emery Berger
-   [Artifact Evaluation: Tips for Authors](https://blog.padhye.org/Artifact-Evaluation-Tips-for-Authors/), by Rohan Padhye
-   [How Are Award-winning Systems Research Artifacts Prepared (Part 1)](https://www.sigops.org/2021/how-are-award-winning-systems-research-artifacts-prepared-part-1/), by Tianyin Xu

# Tips

The following guides will be useful when preparing your artifact:

-   [HOWTO for AEC Submitters](https://docs.google.com/document/d/1pqzPtLVIvwLwJsZwCb2r7yzWMaifudHe1Xvn42T4CcA/edit), by Dan Barowy, Charlie Curtsinger, Emma Tosch, John Vilk, and Emery Berger
-   [Artifact Evaluation: Tips for Authors](https://blog.padhye.org/Artifact-Evaluation-Tips-for-Authors/), by Rohan Padhye

Here are some general tips to make life easier for both artifact authors and evaluators:

-   **Automate as much as possible**, you will save a lot of time in the end from not having to re-run experiments that suffered from human error. This is feasible even for artifacts that need multiple nodes or to replicate configuration in multiple places. See [this repository](https://github.com/SolalPirelli/docker-artifact-eval) for an example of artifact automation with Docker.
    
-   **Try out your own artifact on a blank environment**, following the steps you documented. One lightweight way to do this is to create a Docker container from a base OS image, such as `ubuntu:latest`. You can also use a virtual machine or even provision a real machine if you have the infrastructure to do so.
    
-   **Log both successes and failures**, so that users know that something happened. Avoid logging unnecessary or confusing information, such as verbose output or failures that are actually expected. Log potential issues, such as an optional but recommended library not being present.
    
-   **Measure resource use** using tools such as `mpstat`, `iostat`, `vmstat`, and `ifstat` to measure CPU, I/O, memory, and network use respectively on Linux, or `/usr/bin/time -v` to measures the time and memory used by a command also on Linux. This lets users know what to expect.
    

## Checklists[Permalink](https://secartifacts.github.io/usenixsec2023/tips#checklists "Permalink")

Unfortunately, artifacts sometimes miss badges because they were not tested on a clean setup, or not documented enough, or because running experiments is too error-prone due to complex manual steps. **This year, we provide checklists for authors and evaluators** to help prepare and evaluate artifacts, minimizing the risk of an artifact unnecessarily missing a badge.

### Artifact Available[Permalink](https://secartifacts.github.io/usenixsec2023/tips#artifact-available "Permalink")

-   The artifact is available on a public website with a specific version such as a git commit
-   The artifact has a “read me” file with a reference to the paper
-   Ideally, the artifact should have a license that at least allows use for comparison purposes

Artifacts must meet these criteria _at the time of evaluation_. Promises of future availability, such as artifacts “temporarily” gated behind credentials given to evaluators, are not enough.

### Artifact Functional[Permalink](https://secartifacts.github.io/usenixsec2023/tips#artifact-functional "Permalink")

-   The artifact has a “read me” file with high-level documentation:
    -   A description, such as which folders correspond to code, benchmarks, data, …
    -   A list of supported environments, including OS, specific hardware if necessary, …
    -   Compilation and running instructions, including dependencies and pre-installation steps, with a reasonable degree of automation such as scripts to download and build exotic dependencies
    -   Configuration instructions, such as selecting IP addresses or disks
    -   Usage instructions, such as analyzing a new data set
    -   Instructions for a “minimal working example”
-   The artifact has documentation explaining the high-level organization of modules, and code comments explaining non-obvious code, such that other researchers can fully understand it
-   The artifact contains all components the paper describes using the same terminology as the paper, and no obsolete code/data
-   If the artifact includes a container/VM, it must also contain a script to create it from scratch

Artifacts must be usable on other machines than the authors’, though they may require hardware such as specific network cards. Information such as IP addresses must not be hardcoded.

### Results Reproduced[Permalink](https://secartifacts.github.io/usenixsec2023/tips#results-reproduced "Permalink")

-   The artifact has a “read me” file that documents:
    -   The exact environment the authors used, including OS version and any special hardware
    -   The exact commands to run to reproduce each claim from the paper
    -   The approximate resources used per claim, such as “5 minutes, 1 GB of disk space”
    -   The scripts to reproduce claims are documented, allowing researchers to ensure they correspond to the claims; merely producing the right output is not enough
-   The artifact’s external dependencies are fetched from well-known sources such as official websites or GitHub repositories
    -   Changes to such dependencies should be clearly separated, such as using a patch file or a repository fork with a clear commit history

The amount of manual work, such as writing configuration files, should be reasonably minimized. In particular, there should be no redundant manual steps such as writing the same configuration values in multiple places, as this inevitably leads to human error.

# Evaluator guide

This document is a guide through the artifact evaluation process for evaluators.

If you have general questions, please contact the artifact evaluation chairs. If you have a question about a specific artifact, see below for instructions on asking the authors.

## Your Goal as a Reviewer[Permalink](https://secartifacts.github.io/usenixsec2023/guide#your-goal-as-a-reviewer "Permalink")

The goal of artifact evaluation is to help science by ensuring that published papers are accompanied by high-quality artifacts (e.g., software, hardware, datasets, etc.) that can be reused and extended by others. Authors submit their artifacts (and the artifact appendix) after the camera-ready version has been finalized (possibly in an earlier cycle) and are incentivized to participate through the awarding of badges. Moreover, the best artifacts that excel in all the evaluated dimensions will be rewarded with a Distinguished Artifact Award.

Your main goal is to read the paper and judge how well the artifact matches the expectations set by it. We expect artifacts to be (i) consistent with the paper, (ii) as complete as possible, (iii) documented well, and (iv) easy to reuse for further research.

Keep in mind that all artifacts, reviews, and discussions are confidential. Some artifacts may even contain embargoed material (e.g., exploits) due to vulnerability disclosure. As such, we trust you will treat all the AE material as confidential and also delete the artifact after the evaluation has finished (although most authors will publish the artifact upon publication of the paper).

Also keep in mind that artifact evaluation is a cooperative process. Artifacts that initially do not meet the requirements for badges can still get badges if the authors make necessary improvements in time, and evaluators should provide actionable feedback to enable this. Artifacts should only “miss” badges if there was not enough time to reasonably address the evaluators’ concerns, or if the authors were unresponsive or unreasonable. Note that authors will be able to update their artifacts with no restrictions in response to your comments (e.g., to fix bugs). Authors can submit artifact/appendix updates through external repositories rather than HotCRP. We’ll collect the final appendix (and stable reference) via HotCRP again after finalizing decisions.

The papers under evaluation have already been accepted by the technical program committee, so you do not need to evaluate their scientific soundness. However, if you believe you have found a technical flaw in a paper anyway, contact the artifact evaluation chairs.

## Timeline[Permalink](https://secartifacts.github.io/usenixsec2023/guide#timeline "Permalink")

The bidding deadline is the first important deadline, as it will allow the chairs to distribute artifacts in a way that maximizes evaluator expertise and interest. Bidding maximizes your chances to evaluate artifacts in domains you know about and are interested in.

The “kick the tires” period is when evaluators go through the artifacts to ensure they will be able to properly evaluate them later. It is important to do this as soon as possible, so that authors have enough time to fix big issues if needed.

The reviewing and author discussion period comes next, where evaluators evaluate the artifacts and communicate with the authors to request clarifications/improvements to the artifacts and the appendix. Reviews are due at the end of the period, with individual proposals to award (or not to award) each requested badge.

Afterwards, there is some time to agree on badges before the final deadline. This to ensure that there is time for reviewers to discuss the artifacts that need it as well as time for any extra or late evaluations. Keep in mind that the final deadline for agreeing on badges is strict.

## Communicating with authors[Permalink](https://secartifacts.github.io/usenixsec2023/guide#communicating-with-authors "Permalink")

Artifact evaluation is single-blind, meaning authors do not and must not know who you are so that you can be frank in your assessment. To enable this, all communication between authors and reviewers must be done through HotCRP, not by other means such as email.

Please make sure that in your HotCRP profile, under “Preferences”, the “Send mail” box for “Reviews and comments on authored or reviewed submissions” is checked, so that you are notified of comments on your assigned artifacts from authors and fellow reviewers.

To add a comment on HotCRP, at the bottom of the artifact page, click on the “Add comment” button to show a form, type your comment, and select the right visibility for your comment. Discussion with authors must be “Author discussion”, while discussion with evaluators must be “Reviewer discussion”. For chairs-only comments, you can use “Administrators only”. Leave the second option to “about: submission”.

You can notify a fellow evaluator with an @-mention in a HotCRP comment, as on many other platforms. Type @ and let HotCRP autocomplete the name you want. You can also use the same @-mention mechanism to tag the AEC chairs (@Cristiano Giuffrida @Anjo Vahldiek-Oberwagner) and bring an issue to their attention.

Use “Reviewer discussion” comments to synchronize with your fellow evaluators and ensure the same issue was not raised by another review before.

Authors submit their initial version of the artifact, artifact appendix and any other information needed to evaluate the artifact. You should carefully read these documents and make recommendations to the authors to improve the documentation of the artifact. Any errors you find or missing information should be documented and communicated as early as possible to the authors. They will then update the artifact or appendix. The badge decision is made based on the last submitted version of the artifact and appendix and should be independent of how many problems you ran into or changes were needed.

## Evaluation setups[Permalink](https://secartifacts.github.io/usenixsec2023/guide#evaluation-setups "Permalink")

You can evaluate artifacts on various setups, in order of preference:

-   Your own machine, if the artifact supports it
    -   Even if the artifact requires a particular OS or multiple machines, you may be able to run it locally via Docker (e.g. see [this repo](https://github.com/SolalPirelli/docker-artifact-eval)) or using virtual machines such as with VirtualBox
-   Any servers with beefy/special hardware you may have access to, for artifacts that could benefit from this
-   The artifact authors’ machines, accessed via SSH or such, for artifacts that cannot run anywhere else due to hardware dependencies
-   Commercial clouds such as AWS or Azure, but only if absolutely necessary and the authors are willing to pay for it; in that case, please agree with the authors on a protocol in which you agree to spawn and tear down machines to minimize unnecessary costs.

_Note on anonymization_: If you have to SSH to the authors’ machines, make sure your public SSH key does not identify you (remove the user@host part at the end). If you are concerned you could be identified through other means, such as because of your IP address (e.g., because you do not have access to a VPN), contact the chairs.

## Bidding phase[Permalink](https://secartifacts.github.io/usenixsec2023/guide#bidding-phase "Permalink")

Once artifacts are submitted, you need to bid for the artifacts you want to review. You can enter your preferences by the bidding deadline by logging into HotCRP and clicking on “Review preferences”. You can use -20 to 20 as the range to rank the artifacts by preference and -100 to declare a conflict of interest (contact the AE chairs if unsure). When bidding, also pay attention to the hardware/software requirements of the artifact.

Note: we will try to match artifacts to your preferences, but if you don’t bid by the deadline, you may be assigned less-than-ideal artifact(s) for your profile.

## Initial “kick the tires” phase[Permalink](https://secartifacts.github.io/usenixsec2023/guide#initial-kick-the-tires-phase "Permalink")

Once you have been assigned artifacts comes the initial “kick the tires” period. The goal of this period is to quickly determine whether you have everything you need for a full review: the artifact itself, any necessary hardware or other dependencies, and a plan on how you will evaluate the artifact. If that is not the case, you must discuss with your fellow evaluators and let the authors know of any problems as soon as possible, so that they have enough time to fix issues.

Double-check which badges the authors requested in their artifact submission; you do not need to evaluate the artifact for badges that were not requested (if you believe an artifact already meets the requirements for a badge the authors did not request, ask the authors; they may have forgotten to request that badge).

Carefully read the artifact documentation. In particular, check the software and hardware dependencies to make sure you have all you need. You are allowed to use your own judgment when making decisions, for instance to evaluate reasons why some artifacts may not be able to reproduce everything their paper contains. Before starting the evaluation, consider the following points and ideally share the evaluation plan with the authors:

Before starting the evaluation, consider the following points and ideally share the evaluation plan with the authors:

-   Whether you have everything you need to do the evaluation, and if not, what is missing including:
    -   Access to the necessary hardware owned by you, by the authors
    -   For artifacts requesting the “functional” badge, documentation and full source code as mentioned in [the checklist](https://secartifacts.github.io/usenixsec2023/tips#artifact-functional), and whether the code compiles
    -   For artifacts requesting the “reproduced” badge, additionally the scripts to run the experiments and generate figures as mentioned in [the checklist](https://secartifacts.github.io/usenixsec2023/tips#results-reproduced)
-   A plan on how you will evaluate the artifact during the review period: s * Time frames of when experiments will be run in case hardware is shared

## Reviewing artifacts[Permalink](https://secartifacts.github.io/usenixsec2023/guide#reviewing-artifacts "Permalink")

For each artifact you are assigned to, you will produce one review explaining which badges you believe should be awarded and why or why not. You will work with the authors to produce your review, as this is a cooperative process. Authors are a resource you can use, exclusively through HotCRP, if you have trouble with an artifact or if you need more details about specific portions of an artifact.

There is an example review at the end of this guide.

First, (re-)read the [page on badges](https://secartifacts.github.io/usenixsec2023/badges).The checklists are particularly important: artifacts that meet these requirements should get the corresponding badges, while artifacts that do not should either justify why or not get the badges. If an artifact does not satisfy a checklist but the authors provide a good reason as to why they should get the badge anyway, use your judgment based on the definitions of the badges. Remember that the Artifacts Functional and Results Reproduced badges require not only running the code but also auditing it to ensure that (for Artifacts Functional) the code is documented and understandable, and (for Results Reproduced) the code actually does what the paper states it does and reproduces results to support all the main claims of the paper (which must be documented in the submitted artifact appendix). Merely reproducing similar output as the paper, such as performance metrics, is not enough, the artifact must actually do what it claims to do. You are not expected to understand every single line of code, but you should be confident that the artifact overall matches the paper’s description.

**Most of your time should be spent auditing artifacts, not debugging them**. If you run into issues such as missing dependencies, try to quickly work around them, such as by finding the right package containing the dependency for your operating system and letting the authors know they have to fix their instructions. However, it is the authors’ responsibility to make their artifacts work, not yours. You do not need to spend hours trying to debug and fix complex issues; if you encounter a non-trivial error, first ask your fellow evaluators if they encountered it too or if they know how to fix it, then ask the authors to fix it.

**It is acceptable to deny badges if artifacts require unreasonable effort**, especially if such effort could be avoided through automation. For instance, if reproducing a claim requires 50 points of data, and the artifact requires you to manually edit 5 config files then run 4 commands on 3 machines for each data point, you do not need to actually perform hundreds of manual steps; instead, ask the authors to automate this, or even write a script yourself if you have the time that you can then share with the authors.

Concerning the artifact appendix, please verify it follows the provided [template](https://secartifacts.github.io/usenixsec2023/instructions#artifact-appendix) and its constraints (mandatory sections in particular). Do ask the authors for updates during the review process if the appendix does not follow the template or if important information is missing. Similarly, if authors apply for the Artifacts Available badge, please verify they provided a stable reference (URL) to the artifact at submission time (see [badge](https://secartifacts.github.io/usenixsec2023/badges) requirements for details). If not, do ask for updates during the review process.

Once you are finished evaluating an artifact, fill in the review form and submit it at your earliest convenience. Your review must explain in detail why the artifact should or should not get each of the badges that the authors requested. You can also include additional suggestions for the authors to improve their artifacts if you have any. Note that you can edit your review as many times as you like, since reviews only become visible to the authors when final decisions are announced.

Remember that the artifact evaluation process is cooperative, not adversarial. Give authors a chance to fix issues by discussing through HotCRP comments before deciding that their artifact should not get a badge. In other words, help the authors improve their artifacts and reach badge status in the allocated time, whenever possible. However, if authors are being unresponsive or unreasonable, feel free to post a comment stating a badge cannot be awarded unless the authors take the specified steps in time by the deadline.

HotCRP allows you to rate your fellow evaluators’ reviews. If you think a review is well done, don’t hesitate to add a positive vote! If you think a review could use improvement, you can leave a negative vote and a reviewer discussion comment explaining your thoughts.

## Example review[Permalink](https://secartifacts.github.io/usenixsec2023/guide#example-review "Permalink")

We provide here an example review for a fictitious artifact/paper. This review started by copy-pasting each point from the badge checklists, then modifying the text to suit the artifact and starting each point with one of ✔ (= yes), ❌ (= no), or ⚠ (= yes, but has issues). For the “Results Reproduced” badges, if results differ from the original in any way it’s good to explain how, even if the badge should be awarded. Remember that on HotCRP you can use Markdown for headings, lists, tables, and so on.

### Artifact Available[Permalink](https://secartifacts.github.io/usenixsec2023/guide#artifact-available "Permalink")

-   ✔ The artifact is available on a public GitHub repository
-   ✔ The artifact has a “read me” file with a reference to the paper
-   ⚠ The artifact does not have a license that allows use for comparison purposes; this is not necessary but it would be good to have

I suggest awarding the badge.

### Artifact Functional[Permalink](https://secartifacts.github.io/usenixsec2023/guide#artifact-functional "Permalink")

-   ❌ The artifact ‘s “read me” file is missing some information:
    -   ✔ It has a description
    -   ✔ It has compilation and running instructions
    -   ✔ It has usage instructions to run experiments
    -   ❌ It does not have a list of supported environments
    -   ❌ It does not have configuration instructions to select the client and server IPs
    -   ❌ It does not have instructions for a “minimal working example”, only for full experiments on 12 machines
-   ✔ The code is well documented at both the module and class level, good job!
-   ⚠ The artifact contains all major parts described in the paper; it would be good if it included the extra experiments mentioned in the paper’s Limitations section as well, but this is not mandatory

I hope authors can fix the issues mentioned above so that the Artifact Functional badge can be awarded.

### Results Reproduced[Permalink](https://secartifacts.github.io/usenixsec2023/guide#results-reproduced "Permalink")

I considered the 3 claims as per the artifact appendix, except for claim #3 in which I used a different configuration file after our discussion with the authors. All experiments were carried out on CloudLab using the authors’ profile. I obtained all software from the artifact’s GitHub repository, commit abc0def.

-   ✔ The artifact has a “read me” file that documents:
    -   ✔ The exact environment the authors used
    -   ✔ The exact commands to run to reproduce each claim from the paper
    -   ⚠ The time used per claim, but not the disk space which would be nice to indicate since it is multiple GBs
    -   ✔ The scripts to reproduce claims are very well documented and correspond to what the paper states

For claim 2, I obtained 4400 ops/s for the artifact and 3500 ops/s for the baseline, which is a bit lower for the artifact than what the paper claims. However, the key part of the claim is that the artifact is at least as fast as the baseline, not an absolute performance number, so I believe this is fine. I suggest awarding the badge.

### Acknowledgements

The AE process at USENIX Security '23 is a continuation of the AE process at USENIX Security '20–'22 and was inspired by multiple other conferences, such as OSDI, EuroSys, and several other systems conferences. See [artifact-eval.org](https://artifact-eval.org/about.html) for the origins of the AE process.
