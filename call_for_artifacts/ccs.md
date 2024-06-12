# Call For Artifacts


A scientific paper consists of a constellation of artifacts that extend beyond the document itself: software, hardware, evaluation data and documentation, raw survey results, mechanized proofs, models, test suites, benchmarks, and so on. In some cases, the quality of these artifacts is as important as that of the document itself. Last year, CCS introduced an artifact evaluation process to promote the development of high-quality artifacts and recognize their authors. Building on last year’s success, CCS will again run an optional artifact evaluation process this year.

The artifact evaluation process will consider the availability and functionality of artifacts associated with their corresponding papers, along with the reproducibility of the paper’s key results and claims with these artifacts. Artifact evaluation is single blind. Artifacts will be held in confidence by the evaluation committee. While the committee strongly encourages the authors of CCS papers to make their artifacts publicly available, the artifact evaluation process is open to artifacts that are not.

All accepted CCS papers are encouraged to participate in artifact evaluation. See [Submitting an Artifact](https://www.sigsac.org/ccs/CCS2024/call-for/call-for-artifacts.html#submitting) for details on the submission process.

Questions about the process can be directed to the CCS [Artifact Evaluation Chair](mailto:eric.eide@utah.edu).

## Artifact Evaluation Overview

### Benefits and Goals

The dissemination of artifacts benefits our science and engineering as a whole. Their availability encourages replicability and reproducibility and enables authors to build on top of each others’ work. It can help more unambiguously resolve questions about cases not considered by the original authors. It also confers direct and indirect benefits to the authors themselves.

The goal of artifact evaluation is to incentivize authors to invest in their broader scientific community by producing artifacts that illustrate their claims, enable others to validate those claims, and accelerate future scientific progress by providing a platform for others to start from. A paper with artifacts that have passed the artifact evaluation process is recognized by badges that appear on the paper’s first page. In addition, a paper with artifacts may include an appendix that details those artifacts, highlighting the importance of those artifacts to the contributions of the work overall.

For each CCS 2024 review cycle, artifact evaluation will begin only after the paper acceptance decisions for that review cycle have been made. Artifact evaluation is optional, although we hope that the authors of all accepted papers will participate.

### Evaluation Criteria and Badges

For each paper with submitted artifacts, members of the Artifact Evaluation Committee (AEC) will read the paper and judge how well the submitted artifacts conform to the expectations set by the paper. In brief, the AEC expects that high-quality artifacts will be:

-   consistent with the paper,
-   as complete as possible,
-   documented well, and
-   easy to reuse, facilitating further research.

At artifact-submission time, a submitter will choose the criteria by which their artifacts will be evaluated. The criteria correspond to three kinds of badges that can be awarded to a paper under the ACM’s [Artifact Review and Badging Policy, Version 1.1](https://www.acm.org/publications/policies/artifact-review-and-badging-current). An artifact can satisfy the criteria of one, two, or all three of the following types of badges:

-   **Artifacts Available.** To earn this badge, the AEC must judge that the artifacts associated with the paper have been made available for retrieval, permanently and publicly. Valid hosting options include institutional repositories and third-party digital repositories _that have a declared plan to enable permanent accessibility_, e.g., [Zenodo](https://zenodo.org/), [FigShare](https://figshare.com/), [Dryad](https://datadryad.org/stash/), or [Software Heritage](https://archive.softwareheritage.org/). **In particular**, making the artifacts available solely through personal web pages, [GitHub](https://github.com/), [GitLab](https://about.gitlab.com/), or a similar software-development site is **not adequate** for receiving this badge. Other than making the artifacts available, this badge does not mandate any further requirements on functionality, correctness, or documentation.
    
-   **Artifacts Evaluated.** To earn this badge, the AEC must judge that the artifacts conform to the expectations set by the paper in terms of functionality, usability, and relevance. In short, do the artifacts work and are they useful for producing outcomes associated with the paper? The AEC will consider four aspects of the artifacts in particular. (i) _Documented:_ are the artifacts sufficiently documented to enable them to be exercised by readers of the paper? (ii) _Consistent:_ are the artifacts relevant to the paper, and do they contribute in some inherent way to the generation of its main results? (iii) _Complete:_ do the submitted artifacts include all of the key components described in the paper? (iv) _Exercisable:_ do the submitted artifacts include the scripts and data needed to run the experiments described in the paper, and can the software be successfully executed? The Artifacts Evaluated badge has two levels. Artifacts that are judged to satisfy the above criteria will be awarded the **Artifacts Evaluated—Functional** badge. Artifacts that are judged to significantly exceed the minimum standards for the above criteria, to the point that the artifacts facilitate reuse and repurposing by others, may instead be awarded the **Artifacts Evaluated—Reusable** badge.
    
-   **Results Reproduced.** To earn this badge, the AEC must judge that they can use the submitted artifacts to obtain the main results presented in the paper. In short, is it possible for the AEC to independently repeat the experiments and obtain results that support the claims made by the paper? The goal of this effort is not to reproduce the results exactly, but instead to generate results independently within an allowed tolerance such that the main claims of the paper are validated.
    

### Process

Authors are invited to submit their artifacts shortly after their papers have been accepted for publication at CCS. For CCS 2024, there are three rounds of artifact evaluation, to accommodate papers that are accepted at different points in time.

-   **First Paper Review Cycle**
    -   If your paper is **accepted**, with or without shepherding, submit your artifact to the First Artifact Review Cycle.
    -   If your paper is accepted after completing **minor revisions**, submit your artifact to the Second Artifact Review Cycle.
-   **Second Paper Review Cycle**
    -   If your paper is **accepted**, with or without shepherding, submit your artifact to the Second Artifact Review Cycle.
    -   If your paper is accepted after completing **minor revisions**, submit your artifact to the Third Artifact Review Cycle.

You must submit your artifacts according to the time that your paper is accepted, as described above. You cannot “postpone” the review of your paper’s artifacts until a later cycle.

Because the time between paper acceptance and artifact submission is short, the Artifact Evaluation Chair encourages authors to starting prepare their artifacts for evaluation while their papers are still under consideration by the Program Committee. See the [guidelines for packaging artifacts](https://www.sigsac.org/ccs/CCS2024/call-for/call-for-artifacts.html#packaging) later in this document.

After each artifact submission deadline, members of the AEC will download each artifact package, read the accepted paper, install the artifacts (where relevant), and finally evaluate the artifacts. AEC members may communicate with artifact authors—through HotCRP to maintain the evaluators’ anonymity—to resolve minor issues and ask clarifying questions. Authors must respond to messages from the AEC in a timely manner for their artifacts to be effectively considered.

The AEC will complete its evaluation and notify authors of the outcomes. Authors can use the time between notification and the camera-ready deadline to incorporate feedback and artifact details into the camera-ready versions of their papers. This is intended to allow authors to include the feedback from the AEC, at their option.

When the AEC judges that an artifact meets the criteria for one or more of the badges listed above, those badges will appear on the final version of the associated paper. In addition, the authors of the paper will be encouraged to add an **Artifact Appendix** to their publication. The goal of the appendix is to describe and document the artifact in a standard format. The template for the appendix will be made available to authors following artifact evaluation.

### Artifact Details

The AEC will try to accept any kind of digital artifact that authors wish to submit: software, datasets, survey results, test suites, mechanized proofs, etc. Paper proofs will not be accepted, because the AEC lacks the time and often the expertise to carefully review paper proofs. Physical objects, e.g., computer hardware, cannot be accepted due to the difficulty of making the objects available to members of the AEC. (If your artifact requires special hardware, consider if/how you can make it available to evaluators online.)

Participating in artifact evaluation does not require you to publish your artifacts (although it is highly encouraged). The submission of an artifact does not give the AEC permission to make its content public. AEC members will be instructed that they may not publicize any part of your artifact during or after completing evaluation, and they will not retain any part of it after evaluation. Thus you are free to include models, data files, proprietary binaries, etc. in your artifact.

Some artifacts may attempt to perform malicious or destructive operations by design. These cases should be boldly and explicitly flagged in detail in the README so the AEC can take appropriate precautions before installing and running these artifacts. Please contact the [Artifact Evaluation Chair](mailto:eric.eide@utah.edu) if you believe that your artifacts fall into this category.

### Review and Anonymity

Artifact evaluation is “single blind.” The identities of artifact authors will be known to members of the AEC, but authors will not know which members of the AEC have reviewed their artifacts.

To maintain the anonymity of artifact evaluators, the authors of artifacts should not embed any analytics or other tracking in the websites for their artifacts for the duration of the artifact-evaluation period. If you cannot control this, do not access this data. This is important to maintain the confidentiality of the evaluators. In cases where tracing is unavoidable, authors should notify the Artifact Evaluation Chair in advance so that AEC members can take adequate safeguards.

## Submitting an Artifact

### Registration and Submission

Be sure to submit your artifacts by the deadline corresponding to when your paper is accepted, as described earlier in this call. You cannot “postpone” the review of your paper’s artifacts until a later cycle/deadline.

Submitting the artifacts associated with your CCS paper is a two-step process.

1.  **Registration.** By the appropriate artifact registration deadline, submit the abstract and PDF of your accepted CCS paper, as well as topics, conflicts, and any “optional bidding instructions” for potential evaluators via the artifact submission site.
    
    -   [First round artifact submission site](https://ccs2024a-artifacts.hotcrp.com/)
    -   _Second round submission site to be announced._
    -   _Third round submission site to be announced._
2.  **Submission.** Follow these steps to complete your artifact submission:
    
    -   By the appropriate artifact submission deadline, provide a stable URL or (if that is not possible) upload an archive of your artifacts.
    -   If the URL is access-protected, provide the credentials needed to access it.
    -   Select the criteria/badges that the AEC should consider while evaluating your artifacts.
    -   **Special note:** For your artifacts be considered for the “Artifacts Available” badge, the URL included in your submission must point to the artifacts in a suitable digital repository: _notably, not GitHub_. See the discussion of [using Zenodo](https://www.sigsac.org/ccs/CCS2024/call-for/call-for-artifacts.html#zenodo), below.
    -   You will not be able to change the URL, archive, or badge selections after the artifact submission deadline.
    -   Finally, for your artifact to be considered, check the “ready for review” box before the submission deadline.

The AEC recommends that you create a single web page at a stable URL that contains your artifact package. (Again, see the discussion of [using Zenodo](https://www.sigsac.org/ccs/CCS2024/call-for/call-for-artifacts.html#zenodo) for this purpose.) The AEC may contact you with questions about your artifacts if your submitted materials are unclear.

### Packaging Artifacts

The goal of the Artifact Evaluation Committee is to judge whether the artifacts that you submit conform to the expectations set by your paper in the context of the criteria associated with the badges you have selected. The effort that you put into packaging your artifacts has a direct impact on the committee’s ability to make well-informed decisions. Please package your artifacts with care to make it as straightforward and easy as possible for the AEC to understand and evaluate their quality.

A complete artifact package must contain:

-   the accepted version of your CCS paper
-   the artifact itself
-   instructions!

Your artifact package must include an obvious “README” that describes your artifact and provides a road map for evaluation. The README should contain or point to **suitable instructions and documentation**, to save committee members the burden of reverse-engineering the authors’ intentions. (A tool without a quick tutorial is generally very difficult to use. Similarly, a dataset is useless without some explanation on how to browse the data.) For software artifacts, the README should—at a minimum—provide instructions for installing and running the software on relevant inputs. For other types of artifacts, describe your artifact and detail how to “use” it in a meaningful way.

Importantly, make your **claims** about your artifacts concrete. This is especially important if you think that these claims differ from the expectations set up by your paper. The AEC is still going to evaluate your artifacts relative to your paper, but your explanation can help to set expectations up front, especially in cases that might frustrate the evaluators without prior notice. For example, tell the AEC about difficulties they might encounter in using the artifact, or its maturity relative to the content of the paper.

Authors should consider using one or more of the following methods to package the software components of their artifacts (although the AEC is open to other reasonable formats as well):

-   **Source code:** If your artifact has few dependencies and can be installed easily on several operating systems, you may submit source code and build scripts. However, if your artifact has a long list of dependencies, please use one of the other formats below.
-   **Container/virtual machine:** A Docker image or virtual machine containing the software application already set up with the right toolchain and intended runtime environment. For example:
    -   For raw data, the container/VM would contain the data and the scripts used to analyze it.
    -   For a mobile phone application, the container/VM would have a phone emulator installed.
    -   For mechanized proofs, the container/VM would contain the right version of the relevant theorem prover.
-   **CloudLab or Chameleon experiment:** [CloudLab](https://www.cloudlab.us/), [Chameleon](https://www.chameleoncloud.org/), and similar platforms provide facilities for packaging entire computational environments and making them accessible to others.
-   **Binary installer:** Indicate exactly which platform and other run-time dependencies your artifact requires.
-   **Live instance on the web:** Ensure that it is available for the duration of the artifact evaluation process.
-   **Internet-accessible hardware:** If your artifact requires special hardware (e.g., SGX or another trusted execution environment), or if your artifact is actually a piece of hardware, please make sure that AEC members can somehow access the device. VPN-based or SSH-based access to the device might be an option.
-   **Screencast:** A detailed screencast of the tool along with the results, especially if one of the following special cases applies:
    -   The artifact needs proprietary/commercial software or proprietary data that is not easily available or cannot be distributed to the committee.
    -   The artifact requires significant computation resources (e.g., more than 24 hours of execution time to produce the results) or requires huge data sets.
    -   The artifact requires specific hardware or software that is not generally available in a typical lab and where no access can be provided in a reasonable way.

As previously described, in all cases, artifacts must be provided in a manner that is appropriate for single-blind review by members of the AEC (i.e., anonymous reviewers).

### Using Zenodo

We recommend that you make your artifacts available to the AEC as a record in Zenodo. _You are not required to use Zenodo,_ but doing so can help you meet the criteria of the “Artifacts Available” badge.

[Zenodo](https://zenodo.org/) is an online archival facility allows scientists to preserve and share digital “records” that contain software, data, and other kinds of documents. A [Zenodo record](https://help.zenodo.org/docs/deposit/about-records/) includes metadata, a collection of files, and a persistent Digital Object Identifier (DOI). Once created, a record cannot be deleted, but its author can create new versions of the record at any time. Together, these properties make Zenodo well suited to the artifact evaluation process.

You can use Zenodo whether or not you intend to make your artifacts publicly available. (To receive the “Artifacts Available” badge, of course, your artifacts must be public.)

-   If you intend to publish your artifacts, which is the preferred option, you can set the visibility of your artifacts’ record to “Public.” Note that this will generate a Zenodo DOI that is permanently public.
    
-   If you do not want to make your artifacts publicly available, you can set the visibility of your artifacts’ record to “Restricted.” You will need to grant access to individual users (in particular, members of the AEC) who want access to your artifacts’ record.
    

Three additional points are worth noting. First, Zenodo has extensive [online documentation](https://help.zenodo.org/docs/). Second, Zenodo provides a [sandbox environment](https://sandbox.zenodo.org/) where you can practice before creating records for your actual artifacts. Third, the [Zenodo application for GitHub](https://docs.github.com/en/repositories/archiving-a-github-repository/referencing-and-citing-content) can greatly ease the task of “exporting” repositories on GitHub to records within Zenodo.

### Further Advice

There are several sources of good advice about preparing artifacts for evaluation. These two are particularly noteworthy:

-   [Artifact Evaluation: Tips for Authors](https://blog.padhye.org/Artifact-Evaluation-Tips-for-Authors/) by Rohan Padhye
-   [HOWTO for AEC Submitters](https://docs.google.com/document/d/1pqzPtLVIvwLwJsZwCb2r7yzWMaifudHe1Xvn42T4CcA/edit) by Dan Barowy, Charlie Curtsinger, Emma Tosch, John Vilk, and Emery Berger

If you have any questions about how best to package your artifact, contact the [Artifact Evaluation Chair](mailto:eric.eide@utah.edu).

## Acknowledgments

The artifact evaluation process at CCS 2024 is a continuation of the process at CCS 2023 and was inspired by the processes at multiple prior conferences including USENIX Security, SOSP, and several ACM SIGPLAN conferences. Visit [artifact-eval.org](https://artifact-eval.org/) for information about the origins of the artifact evaluation process. Visit [secartifacts.github.io](https://secartifacts.github.io/) for a summary of artifact evaluation efforts at many security conferences.
