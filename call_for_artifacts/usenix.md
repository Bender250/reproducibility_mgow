# Evaluation

A scientific paper consists of a constellation of artifacts that extend beyond the document itself: software, hardware, evaluation data and documentation, raw survey results, mechanized proofs, models, test suites, benchmarks, and so on. In some cases, the quality of these artifacts is as important as that of the document itself, yet many of our conferences offer no formal means to submit and evaluate anything but the paper itself. To address this shortcoming, we are running an optional artifact evaluation process, inspired by similar efforts in software engineering and other areas of science. USENIX Security will run an optional artifact evaluation process, inspired by similar efforts in software engineering and other areas of science.



## Artifact Evaluation Information

### Overview

A scientific paper consists of a constellation of artifacts that extend beyond the document itself: software, hardware, evaluation data and documentation, raw survey results, mechanized proofs, models, test suites, benchmarks, and so on. In some cases, the quality of these artifacts is as important as that of the document itself. To emphasize the importance of such artifacts and promote the reproducibility of experimental results, USENIX Security will run its third (optional) AE this year.

### Benefits

We believe the evaluation and dissemination of artifacts benefits our science and engineering as a whole. Their availability improves replicability and reproducibility, and enables authors to build on top of each other's work. It can also help more unambiguously resolve questions about cases not considered by the original authors.

Beyond helping the community as a whole, it confers several direct and indirect benefits to the authors themselves. The most direct benefit is, of course, the recognition that the authors accrue, with the community rewarding artifacts that sometimes take years to build. Another direct benefit is the ability to improve the final version of the paper and of the artifacts based on feedback from the AEC. In addition, the very act of creating a bundle that can be used by the AEC confers several indirect benefits:

-   The same bundle can be distributed to third parties and we believe this will foster science in general. We strongly encourage authors to make the artifacts available such that other researchers can build upon this artifact.
-   A bundle can be used subsequently for later experiments (e.g., on new parameters or for responding to a journal reviewer's questions).
-   The bundle is more likely to survive being put in storage between the departure of one student and the arrival of the next.

However, creating a bundle that meets all these properties can be onerous. Therefore, the process we describe below does not require an artifact to have all these properties, it offers a route to evaluation that confers fewer benefits for proportionally less effort.

The process is based on experience collected at other venues that have organized such an evaluation process for several years.

The Artifact Evaluation Committee will also grant Distinguished Artifact Awards to outstanding artifacts accepted to USENIX Security 2022.

### Process

To maintain a wall of separation between paper review and the artifacts, authors will be given the option to submit their artifacts only after their papers have been (conditionally) accepted for publication at USENIX Security. The new process for the 2022 Artifact Evaluation edition gives authors 5-6 weeks after the notification to prepare their artifacts. Of course, they can (and should!) prepare their artifacts well in advance, and can already provide the artifacts to the PC via supplemental materials, as many authors already do.

At artifact-submission time, the authors choose the criteria by which their artifacts will be evaluated. The criteria correspond to [**three separate badges**](https://www.usenix.org/conference/usenixsecurity22/call-for-artifacts#badges) that can be awarded to a paper. In general, good artifacts are expected to be: consistent with the paper, as complete as possible, documented well, and easy to (re)use. The AEC will read the paper and then judge if the artifact meets the criteria for each of the requested badges.

Each artifact submission will be reviewed by at least two AEC members. Since we anticipate small glitches with installation and use, reviewers may communicate with authors for a period of three weeks to help resolve glitches while preserving reviewer anonymity. The AEC will then complete its evaluation and notify the authors of the outcome. Please make sure that at least one of the authors is reachable to answer questions in a timely manner.

As the notification of the Artifact Evaluation is after the final paper deadline, badges cannot directly appear on the published papers. Nevertheless, authors are given the possibility to add the awarded badges and the [Artifact Appendix](https://www.usenix.org/sites/default/files/conference-files/sec22_ae_appendix_template_v20220119.zip) on the author version PDF that they can later host on their website or an archive. Moreover, USENIX will publish the badges and the appendices on the conference website. Finally, the badges and the artifact appendices will also be published by USENIX after the conference in dedicated proceedings.

### Badges

Authors can request their artifact to be evaluated towards one, two, or all three of the following badges:

-   **Artifacts Available:** To earn this badge, the AEC must judge that the artifacts associated with the paper have been made available for retrieval, permanently and publicly. We encourage authors to use [Zenodo](https://zenodo.org/), which is a publicly-funded long-term storage platform that also assigns a DOI for your artifact. Other valid hosting options include institutional repositories and third-party digital repositories (e.g., [FigShare](https://figshare.com/), [Dryad](https://datadryad.org/stash/), [Software Heritage](https://archive.softwareheritage.org/), [GitHub](https://github.com/), or [GitLab](https://about.gitlab.com/)—not personal web pages). For repositories that can evolve over time (e.g., GitHub), a stable reference to the evaluated version (e.g., a URL pointing to a commit hash or tag) is required. Note that the stable reference provided at submission time is for the purpose of Artifact Evaluation. Since the artifact can potentially evolve during the evaluation to address feedback from the reviewers, another (potentially different) stable reference will be later collected for the final version of the artifact. Other than making the artifacts available, this badge does not mandate any further requirements on functionality, correctness, or documentation.
-   **Artifacts Functional:** To earn this badge, the AEC must judge that the artifacts conform to the expectations set by the paper in terms of functionality, usability, and relevance. In short, do the artifacts work and are they useful for producing outcomes associated with the paper? The AEC will consider three aspects of the artifacts in particular.

1.  **Documentation:** are the artifacts sufficiently documented to enable them to be exercised by readers of the paper?
2.  **Completeness:** do the submitted artifacts include all of the key components described in the paper?
3.  **Exercisability:** do the submitted artifacts include the scripts and data needed to run the experiments described in the paper, and can the software be successfully executed?

-   **Results Reproduced:** To earn this badge, the AEC must judge that they can use the submitted artifacts to obtain the main results presented in the paper. In short, is it possible for the AEC to independently repeat the experiments and obtain results that support the main claims made by the paper? The goal of this effort is not to reproduce the results exactly, but instead to generate results independently within an allowed tolerance such that the main claims of the paper are validated.

### Artifact Details

To avoid excluding some papers, the AEC will try to accept any artifact that authors wish to submit. These can be software, hardware, data sets, survey results, test suites, mechanized proofs, access to special hardware, and so on. Given the experience in other communities, we decided to not accept paper proofs in the artifact evaluation process. The AEC lacks the time and often the expertise to carefully review paper proofs. Obviously, the better the artifact is packaged, the more likely the AEC can actually work with it during the evaluation process.

While we encourage open research, submission of an artifact does not contain tacit permission to make its content public. All AEC members will be instructed that they may not publicize any part of your artifact during or after completing evaluation, nor retain any part of it after evaluation. Thus, you are free to include models, data files, proprietary binaries, exploits under embargo, etc. in your artifact. Also note that participating in the AE does not require you to later publish your artifacts, but of course we strongly encourage you to do so.

In addition, we encourage that you anonymize any data files that you submit. We recognize that some artifacts may attempt to perform malicious operations by design. These cases should be boldly and explicitly flagged in detail in the readme so AEC members can take appropriate precautions before installing and running these artifacts. The evaluation of exploits and similar results might lead to additional hurdles where we still need to collect experience on how to handle this best. Please contact us in case you have concerns, for example when evaluating bug finding tools or other types of artifacts that need special requirements.

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

### Acknowledgements

The AE process at USENIX Security '22 is a continuation of the AE process at USENIX Security '20 and '21 and was inspired by multiple other conferences, such as OSDI, EuroSys, and several other systems conferences. See [artifact-eval.org](https://artifact-eval.org/about.html) for the origins of the AE process.
