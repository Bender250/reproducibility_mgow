
## PoPETs Artifact Review

PoPETs reviews and publishes digital artifacts related to its accepted papers. This process aids in the reproducibility of results and allows others to build on the work described in the paper. Artifact submissions are requested from authors of all accepted papers, and although they are optional, we strongly encourage you to submit your artifacts for review.

Possible artifacts include (but are not limited to):

-   Source code (e.g., system implementations, proof of concepts)
-   Datasets (e.g., network traces, raw study data)
-   Scripts for data processing or simulations
-   Machine-generated proofs
-   Formal specifications
-   Build environments (e.g., VMs, Docker containers, configuration scripts)

Artifacts are evaluated by the [artifact review committee](https://petsymposium.org/artifacts.php#committee). The committee evaluates the artifacts to ensure that they provide an acceptable level of utility, and feedback is given to the authors. Issues considered include software bugs, readability of documentation, and appropriate licensing. After your artifact has been approved by the committee, we will accompany the paper link on [petsymposium.org](https://petsymposium.org/) with a link to the artifact along with an artifact badge so that interested readers can find and use your hard work.

### Artifact Submission Guidelines

-   All submitted artifacts should be relevant to their corresponding PoPETs paper. Please provide a copy of your paper or a brief description of how the artifact is relevant to it in your submission.
-   Many papers have several artifacts (e.g., multiple source code repositories, datasets, build environments), which is great! Please keep in mind that we'll need a single link to put on the PETS website and that all artifacts associated with your paper should be discoverable from that link.
-   All submitted artifacts should be submitted by providing a link to where the artifacts are publicly hosted. Valid hosting options are institutional and third-party digital repositories. Please do not use personal web pages. The link should be persistent; for repositories that evolve over time (e.g., Git repositories), please specify a specific commit-id or tag to be evaluated.
-   Please include a README with your submission that briefly explains the type and purpose of the artifact (e.g., whether it's a proof of concept implementation, scripts for generating graphs, or datasets for reproducing results).
-   All artifacts must be immediately available to the public and **should not** be behind any kind of paywall or restricted access. If the artifact requires you as an author to manually approve requests for access, it is not public and will not qualify as a PoPETs artifact submission. If you have concerns or questions about this please contact us directly.

#### Source Code Submissions

-   All source code should be accompanied by a README or other documentation that describes how to build and/or run the code. Reviewers will provide feedback on the clarity of the instructions and attempt to follow them and build and/or run the code.
-   Any source code submissions should be accompanied with a build environment such as a virtual machine (recommended) or a Docker container that has been configured with all the dependencies and prerequisites necessary to build the code.
-   If you use a virtual machine, please state how many resources it will consume and any configuration steps that are required. Your virtual machine should not usually have to download additional dependencies when you run your install scripts. If that is the case, reassess your build process and consider making changes to limit the amount of network resources needed.
-   If the code is in a compiled language, the code should compile in the provided build environment by performing the provided instructions.
-   If the code is interpreted, please provide some simple inputs so that the reviewers can verify that the code runs without error. We want to make sure that the code will execute without error, not that the outputs are necessarily correct.
-   Compilation and setup should be automated as much as possible. Ideally, there will be one script that builds your software and runs your tests.
-   Please ensure your code has an open source license and clearly states this information. The following resources may help you to choose a license:
    -   For a clear, easy to follow guide see: [https://choosealicense.com/](https://choosealicense.com/)
    -   For more in-depth detail on open source and copy-left licenses, see [https://www.gnu.org/licenses/license-list.en.html](https://www.gnu.org/licenses/license-list.en.html) and [https://opensource.org/licenses](https://opensource.org/licenses)
-   Our goal with these artifacts is for them to be useful as far into the future as possible. Some tips on improving the longevity of your source code artifact are:
    -   Include the versions of your software's dependencies wherever possible
    -   Mention specific hashes of git commits that match the state your artifact was in at the time of submission
    -   Virtual machines will last longer than Docker files and allow researchers to more accurately reproduce your exact execution environment (though the tradeoff is that they will be larger)
-   Artifacts are **not** required to be able to run on all hardwares and OSes. If your artifact requires any particular hardware / OS, please make it clear in the submission.

#### Dataset Submissions

-   All datasets should be clearly documented in a way that would allow researchers working on similar problems to re-use the dataset for their work.
-   If the dataset includes survey results, please provide a copy of the original survey. This is vital for replication studies and helping researchers interpret the context of your results.
-   If the dataset is very large (> 10 MB) please state so in the README or documentation.
-   It's encouraged to accompany the data with processing scripts that produce any graphs or statistical output that appear in the paper.

### Artifact Badges

For PETS 2024, each accepted artifact will be granted one of the following two badges. During the submission, the authors must select which badge they want their artifacts to be evaluated against.

#### Artifacts Available

This "Available" badge indicates that the artifacts are publicly available at a permanent location with clear documentation on how it relates to the corresponding paper and, if applicable, how to execute the artifact/evaluation without execution error. This badge does *not* mean that the reviewers have reproduced the results. Authors whose artifacts require extremely specialized hardware or software are encouraged to choose this option. Similarly, authors whose artifacts are "not reproducible" (e.g., outcomes of surveys) should also select this option.

#### Artifacts Reproduced

The "Reproduced" badge indicates everything the "Available" badge does and, in addition, that the submitted artifacts reproduce the main findings of the paper. Note that this does not necessarily cover all experiments/data presented in the paper. To submit artifacts for this badge, the authors must specify the commands to run the artifacts clearly and describe how to reproduce each main finding of the paper. Also, they must highlight which results of the paper are not reproducible with the given artifacts. The artifact's quality, structure, and documentation must allow the reviewers to check whether the artifact works as claimed in the paper. Even if the authors choose this option, the review committee may request to grant only an "available" badge if the reviewers cannot reproduce the results (e.g., lack of computational resources).

### What we expect from the authors of artifact submissions

To ensure a smooth submission process, please follow these important guidelines. Firstly, authors should fill out the [template.md](https://petsymposium.org/files/template.md) file provided and include it in their artifacts. This will help the reviewer better understand your work and ensure a seamless review process. Secondly, prompt communication is essential. Authors are kindly requested to respond to reviews and comments within a time span of two weeks. This will facilitate constructive discussions and allow for timely feedback incorporation. Lastly, in the event that changes are requested during the review process, we kindly ask authors to endeavor to incorporate them, at least partially, within two weeks after the request. Your cooperation in adhering to these guidelines will greatly contribute to the efficiency and effectiveness of our submission and review process. We eagerly anticipate receiving your high-quality contributions and look forward to showcasing your research!

### What Makes a Good Review

The goal of artifact review is to help ensure the artifacts are as useful as possible. Towards this goal, the review should check for the following points.

-   Is the artifact publicly available at a permanent location?
-   Documentations:

-   Is the relationship between the artifact and the paper clear?
-   If applicable, is the requirement for running the artifact clear?
-   If applicable, are the instructions to run the artifact sufficient?
-   If applicable, are the required dataset & packages publicly available?

-   Reproducibility: In case that the authors choose "artifact reproduced" badge option, the reviewers should also check that the experiments run and the results displayed are similar to the ones in the paper.

Artifact review process is interactive and we expect the authors to take into account the reviewers' comments and modify their artifacts accordingly. As such, the reviews should contain sufficient details for the authors to make the appropriate changes; for example, if the code fails, then the review should include the environment that it is run on and the error messages. After the authors have fixed the issues, they will add a comment on the submission site, at which point the reviewers can either approve the artifact or provide additional comments for another round of revision.
