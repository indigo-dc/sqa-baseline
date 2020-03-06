---
author-meta:
- Pablo Orviz
- Alvaro Lopez
- Doina Cristina Duma
- Mario David
- Jorge Gomes
- Giacinto Donvito
date-meta: '2020-03-06'
keywords:
- research software
- software quality assurance
- software lifecycle
- devops
- software automation
- software quality baseline
- software testing
- software deployment
- agile development
lang: en-US
title: A set of Common Software Quality Assurance Baseline Criteria for Research Projects
...



<br>
![](images/logo-SYNERGY.png){height="50px"}&nbsp;&nbsp;&nbsp;&nbsp;
![](images/logo-DEEP.png){height="50px"}&nbsp;&nbsp;&nbsp;&nbsp;
![](images/logo-INDIGO.png){height="50px"}&nbsp;&nbsp;&nbsp;&nbsp;
![](images/logo-XDC.png){height="50px"}

_A DOI-citable version of this manuscript is available at <http://hdl.handle.net/10261/160086>_.


<small><em>
This manuscript
([permalink](https://indigo-dc.github.io/sqa-baseline/v/d2b752d9acc5a660643f6577ac6b16264673590b/))
was automatically generated
from [indigo-dc/sqa-baseline@d2b752d](https://github.com/indigo-dc/sqa-baseline/tree/d2b752d9acc5a660643f6577ac6b16264673590b)
on March 6, 2020.
</em></small>

## Authors



+ **Pablo Orviz**<br>
    ![ORCID icon](images/orcid.svg){.inline_icon}
    [0000-0002-2473-6405](https://orcid.org/0000-0002-2473-6405)
    · ![GitHub icon](images/github.svg){.inline_icon}
    [orviz](https://github.com/orviz)<br>
  <small>
     Spanish National Research Council (CSIC); Institute of Physics of Cantabria (IFCA)
  </small>

+ **Alvaro Lopez**<br>
    ![ORCID icon](images/orcid.svg){.inline_icon}
    [0000-0002-0013-4602](https://orcid.org/0000-0002-0013-4602)
    · ![GitHub icon](images/github.svg){.inline_icon}
    [alvaro.lopez](https://github.com/alvaro.lopez)<br>
  <small>
     Spanish National Research Council (CSIC); Institute of Physics of Cantabria (IFCA)
  </small>

+ **Doina Cristina Duma**<br>
    ![ORCID icon](images/orcid.svg){.inline_icon}
    [0000-0002-0124-4870](https://orcid.org/0000-0002-0124-4870)
    · ![GitHub icon](images/github.svg){.inline_icon}
    [caifti](https://github.com/caifti)<br>
  <small>
     National Institute of Nuclear Physics (INFN)
  </small>

+ **Mario David**<br>
    ![ORCID icon](images/orcid.svg){.inline_icon}
    [0000-0003-1802-5356](https://orcid.org/0000-0003-1802-5356)
    · ![GitHub icon](images/github.svg){.inline_icon}
    [mariojmdavid](https://github.com/mariojmdavid)<br>
  <small>
     Laboratory of Instrumentation and Experimental Particle Physics (LIP)
  </small>

+ **Jorge Gomes**<br>
    ![ORCID icon](images/orcid.svg){.inline_icon}
    [0000-0002-9142-2596](https://orcid.org/0000-0002-9142-2596)
    · ![GitHub icon](images/github.svg){.inline_icon}
    [jorge-lip](https://github.com/jorge-lip)<br>
  <small>
     Laboratory of Instrumentation and Experimental Particle Physics (LIP)
  </small>

+ **Giacinto Donvito**<br>
    ![ORCID icon](images/orcid.svg){.inline_icon}
    [0000-0002-0628-1080](https://orcid.org/0000-0002-0628-1080)<br>
  <small>
     National Institute of Nuclear Physics (INFN)
  </small>



## Abstract {.page_break_before}

The purpose of this document is to define a set of quality standards,
procedures and best practices to conform a Software Quality Assurance plan to
serve as a reference within the European research ecosystem related projects
for the adequate development and timely delivery of software products.


## Copyright Notice

Copyright © Members of the INDIGO-DataCloud, DEEP Hybrid-DataCloud and eXtreme
DataCloud collaborations, 2015-2020.

## Acknowledgements

The INDIGO-DataCloud, DEEP-Hybrid-DataCloud, eXtreme-DataCloud and
EOSC-Synergy projects have received funding from the European Union’s 
Horizon 2020 research and innovation programme under grant agreement 
number 653549, 777435, 777367 and 857647 respectively.
<p align="center">
  <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcT1WF4g5KH3PnQE_Ve10QFRS-gZ0NpCQ7Qr-_km1RqnOCEF1fQt">
</p>


## Document Log

| Issue | Date | Comment |
|----------|----------|----------|
| v1.0 | 31/01/2018 | First draft version |
| v2.0 | 05/02/2018 | Updated criteria |
| v3.0 | 20/12/2019 | Code management section, metadata for software |
| v3.1 | 05/03/2020 | Add tags/names for each criteria |


## Introduction and Purpose

This document has been tailored upon the recommendations and requirements found
in the Initial Plan for Software Management and Pilot Services deliverable
@5VMJDbB2,
produced by the INDIGO-DataCloud project. These guidelines evolved throughout
the project’s lifetime and are being extended in the
EOSC-Synergy, DEEP-Hybrid-DataCloud and eXtreme DataCloud subsequent projects. The result is
a consolidated Software Quality Assurance (SQA) baseline criteria emanated
from the European Open Science Cloud (EOSC), which aims to outline the SQA
principles to be considered in the upcoming software development efforts within
the European research community, and continuously evolve in order to be aligned
with future software engineering practices and security recommendations.


## Goals

1. Set the base of minimum SQA criteria that a software developed within EOSC
development project SHOULD fulfill.
2. Enhance the visibility, accessibility and distribution of the produced
source code through the alignment to the Open Source Definition.
3. Promote code style standards to deliver good quality source code emphasizing
its readability and reusability.
4. Improve the quality and reliability of software by covering different
testing methods at development and pre-production stages.
5. Propose a change-based driven scenario where all new updates in the source
code are continuously validated by the automated execution of the relevant
tests.
6. Adopt an agile approach to effectively produce timely and audience-specific
documentation.
7. Lower the barriers of software adoption by delivering quality documentation
and the utilization of automated deployment solutions.
8. Encourage secure coding practices and security static analysis at the
development phase while providing recommendations on external security
assessment.


## Notational Conventions

The keywords “MUST”, “MUST NOT”, “REQUIRED”, “SHALL”, “SHALL NOT”, “SHOULD”,
“SHOULD NOT”, “RECOMMENDED”, “MAY”, and “OPTIONAL” in this document are to be
interpreted as described in RFC 2119 @Ms8G1A12.


## Quality Criteria

The following sections describe the quality conventions and best practices that
apply to the development phase of a software component within the EOSC
ecosystem. These guidelines ruled the software development process of the
former European Commission-funded project INDIGO-DataCloud, where they have
proved valuable for improving the reliability of software produced in the
scientific European arena.

The next sections describe the development process driven by a change-based
strategy, followed by a continuous integration approach. Changes in the source
code, trigger automated builds to analyze the new contributions in order to
validate them before being added to the software component code base.
Consequently, software components are more eligible for being deployed in
production infrastructures, reducing the likelihood of service disruption.

### Code Accessibility [QC.Acc]

* **[QC.Acc01]** Following the open-source model, the source code being produced MUST be open
  and publicly available to promote the adoption and augment the visibility of
  the software developments.
* **[QC.Acc02]** Source code MUST use a Version Control System (VCS).
  * **[QC.Acc02.1]** It is RECOMMENDED that all software components delivered by the same
    project agree on a common VCS.
* **[QC.Acc03]** Source code produced within the scope of a broader development project
  SHOULD reside in a common organization of a version control repository
  hosting service.

### Licensing [QC.Lic]

* **[QC.Lic01]** As open-source software, source code MUST adhere to an open-source license
  to be freely used, modified and distributed by others.
  * **[QC.Lic01.1]** Non-licensed software is exclusive copyright by default.
* **[QC.Lic02]** License MUST be compliant with the Open Source Definition @HdIbF8WL.
  * **[QC.Lic02.1]** RECOMMENDED licenses are listed in the Open Source Initiative portal
    under the Popular Licenses category @xVJMmGVr.
* **[QC.Lic03]** Licenses MUST be physically present (e.g. as a LICENSE file) in the root of
  all the source code repositories related to the software component.

### Code Workflow [QC.Wor]

A change-based approach is accomplished with a branching model.

* **[QC.Wor01]** The main branch in the source code repository MUST maintain a working state
  version of the software component.
  * **[QC.Wor01.1]** Main branch SHOULD be protected to disallow force pushing, thus
    preventing untested and unreviewed source code from entering the
    production-ready version.
  * **[QC.Wor01.2]** New features SHOULD only be merged in the main branch whenever the SQA
    criteria is fulfilled.
* **[QC.Wor02]** New changes in the source code MUST be placed in individual branches.
  * **[QC.Wor02.1]** It is RECOMMENDED to agree on a branch nomenclature, usually by
    prefixing, to differentiate change types (e.g. feature, release, fix).
* **[QC.Wor03]** The existence of a secondary long-term branch that contains the changes for
  the next release is RECOMMENDED.
  * **[QC.Wor03.1]** Next release changes come from the individual branches.
  * **[QC.Wor03.2]** Once ready for release, changes in the secondary long-term branch are
    merged into the main branch and versioned. At that point in time, main
    and secondary branches are aligned. This step SHOULD mark a production
    release.
* **[QC.Wor04]** Semantic Versioning @13UfgtMhu specification is RECOMMENDED for
  tagging the production releases.

### Code Management [QC.Man]

* **[QC.Man01]** An issue tracking system facilitates structured software development. Leveraging
  issues to track down both new enhancements and defects (bugs or documentation typos) 
  is RECOMMENDED.
  * **[QC.Man01.1]** In addition to monitoring the internal development, issues are the best means for
    supporting users. External users SHOULD be able to create incidences based on the
    operational performance of the software.
  * **[QC.Man01.2]** The description of an issue SHOULD be concise and state clearly the problem. It is 
    RECOMMENDED to add any reference to the actual problem. In the case of bugs, the 
    issue SHOULD be accompanied by the relevant debug information.
         * The usage of templates for the issue description is RECOMMENDED.
* **[QC.Man02]** In social coding environments, pull requests represent the cornerstone of collaboration. 
  A pull request provides a place for review and discussion of the changes proposed to be
  part of an existing version of the code.
  * **[QC.Man02.1]** Pull requests SHOULD be used for every change in the codebase.
  * **[QC.Man02.2]** A software project SHOULD be open to external collaboration through pull requests.
  * **[QC.Man02.3]** A pull request description SHOULD be concise and state clearly its purpose (e.g. if
    it is fixing an observed bug or adding a new feature)
    * The usage of templates for the pull request's description is RECOMMENDED.
  * **[QC.Man02.4]** It is RECOMMENDED to use pull requests to address open issues. The pull request 
    description SHOULD make reference to the identifiers of the issues it is fixing 
    (to eventually close them, either manually or automatically).

### Code Style [QC.Sty]

Code style requirements pursue the correct maintenance of the source code by
the common agreement of a series of style conventions. These vary based on the
programming language being used.

* **[QC.Sty01]** Each individual software product MUST comply with community-driven or de-facto
  code style standards for the programming languages being used.
  * **[QC.Sty01.1]** Compliance with multiple complementary standards MAY exist.
* **[QC.Sty02]** Custom code style guidelines SHOULD be avoided, only considered in the
  hypothetical event of programming languages without existing community style
  standards.
  * **[QC.Sty02.1]** Custom styles MUST be documented by defining each convention and its
    expected output.
  * **[QC.Sty02.2]** Custom styles SHOULD evolve over time towards a more consistent
    definition.
* **[QC.Sty03]** Exceptions of individual conventions from the main definition are allowed
  but SHOULD bavoided
  * **[QC.Sty03.1]** Absence of standard conventions SHOULD be justified and tracked.
* **[QC.Sty04]** Code style compliance testing MUST be automated and MUST be triggered for
  each candidate change in the source code.

### Code metadata [QC.Met]

Metadata for the software component provides a way to achieve its full identification,
thus making software citation viable [@AJBpTuJY].
It allows the assignement of a Digital Object Identifier (DOI) and is key
towards preservation, discovery, reuse, and attribution of the software component.

* **[QC.Met01]** A metadata file SHOULD exist along side the code, under its VCS.
  The metadata file SHOULD be updated when needed, as is the case of a new version.

### Unit Testing [QC.Uni]

Unit testing evaluates all the possible flows in the internal design of the
code, so that its behaviour becomes apparent. It is a key type of testing for
early detection of failures in the development cycle.

* **[QC.Uni01]** Minimum acceptable code coverage threshold SHOULD be 70%.
  * **[QC.Uni01.1]** Unit testing coverage SHOULD be higher for those sections of the code
    identified as critical by the developers, such as units part of a
    security module.
  * **[QC.Uni01.2]** Unit testing coverage MAY be lower for external libraries or pieces of
    code not maintained within the product’s code base.
* **[QC.Uni02]** Units SHOULD reside in the repository code base but separated from the main
  code.
* **[QC.Uni03]** Unit testing coverage MUST be checked on change basis.
* **[QC.Uni04]** Unit testing coverage MUST be automated.
  * **[QC.Uni04.1]** When working on automated testing, the use of testing doubles is
    RECOMMENDED to mimic a simplistic behaviour of objects and procedures.

### Functional Testing [QC.Fun]

Functional testing involves the verification of the software component’s
identified functionality, based on requested requirements and agreed design
specifications. This type of software testing focus on the evaluation of the
functionality that the software component exposes, leaving apart any internal
design analysis or side-effects to external systems.

* **[QC.Fun01]** Functional testing SHOULD tend to cover the full set of functionality that
  the software component claims to provide.
* **[QC.Fun02]** Functional tests SHOULD be checked automatically with the exception of those
  functionality that require human interaction, such as Graphical User
  Interfaces (GUI).
* **[QC.Fun03]** When working on automated testing, the use of testing doubles is RECOMMENDED
  to mimic a simplistic behaviour of objects and procedures.
* **[QC.Fun04]** Functional tests SHOULD reside in the software component repository code
  base but separated from the main code.
* **[QC.Fun05]** Regression testing, that checks the conformance with previous tests, is
  covered at this stage by executing the complete set of functional tests
  available.
* **[QC.Fun06]** Functional and regression testing MUST be checked on change basis.
* **[QC.Fun07]** Functional and regression testing coverage MAY NOT be suitable for automated
  testing.

### Integration Testing [QC.Int]

Integration testing refers to the evaluation of the interactions among coupled
software components or parts of a system that cooperate to achieve a given
functionality.

* **[QC.Int01]** Integration testing outcome MUST guarantee the overall operation of the
  software component whenever new functionality are involved.
* **[QC.Int02]** Integration testing MAY be complemented with Acceptance and Scalability
  testing.
* **[QC.Int03]** Integration testing MAY NOT be suitable for automated testing.
* **[QC.Int04]** Ad-hoc pilot service infrastructures and/or local testbeds MAY be used to 
  cope with the integration testing requirements.
* **[QC.Int05]** Integration testing MAY NOT be viable to be checked on change basis, as it
  is likely to involve complex scenarios.

### Documentation [QC.Doc]

* **[QC.Doc01]** Documentation MUST be treated as code.
  * **[QC.Doc01.1]** Version controlled, it MAY reside in the same repository where the source
    code lies.
* **[QC.Doc02]** Documentation MUST use plain text format using a markup language, such as
  Markdown or reStructuredText.
  * **[QC.Doc02.1]** It is RECOMMENDED that all software components delivered by the same
    project agree on a common markup language.
* **[QC.Doc03]** Documentation MUST be online available in a documentation repository.
  * **[QC.Doc03.1]** Documentation SHOULD be rendered automatically.
* **[QC.Doc04]** Documentation MUST be updated on new software versions involving any
  substantial or minimal change in the behaviour of the application.
* **[QC.Doc05]** Documentation MUST be updated whenever reported as inaccurate or unclear.
* **[QC.Doc06]** Documentation MUST be produced according to the target audience, varying
  according to the software component specification. The identified types of
  documentation and their RECOMMENDED content are:
  * **[QC.Doc06.1]** README file
    * One-paragraph description of the application.
    * A “Getting Started” step-by-step description on how to get a
      development environment running (prerequisites, installation).
    * Automated test execution how-to.
    * Links to the external documentation below (production deployment,
      user guides).
    * Contributing code of conduct (optionally linked to an external
      CONTRIBUTING file)
    * Versioning specification.
    * Author list and contacts.
    * License information, with a link to the detailed description in an
      external LICENSE file.
    * Acknowledgments.
  * **[QC.Doc06.2]** Developer
    * Private API documentation.
    * Structure and interfaces.
    * Build documentation.
  * **[QC.Doc06.3]** Deployment and Administration
    * Installation and configuration guides.
    * Service Reference Card, with the following RECOMMENDED content:
    * Brief functional description.
    * List of processes or daemons.
    * Init scripts and options.
    * List of configuration files, location and example or template.
    * Log files location and other useful audit information.
    * List of ports.
    * Service state information.
    * List of cron jobs.
    * Security information.
    * FAQs and troubleshooting.
  * **[QC.Doc06.4]** User
    * Public API documentation.
    * Command-line (CLI) reference.
* **[QC.Doc07]** Documentation MUST be checked on change basis.

### Security [QC.Sec]

* **[QC.Sec01]** Secure coding practices SHALL be applied into all the stages of a software
  component development lifecycle.
  * **[QC.Sec01.1]** Compliance with Open Web Application Security Project (OWASP) secure
    coding guidelines @13kp1l5RC
    is RECOMMENDED, even for non-web applications.
* **[QC.Sec02]** Source code SHALL use automated linter tools to perform static application
  security testing (SAST) @18kdpX8Tx
  that flag common suspicious constructs that may cause a bug or lead to a
  security risk (e.g. inconsistent data structure sizes or unused resources).
* **[QC.Sec03]** Dynamic application security testing (DAST) @WzDw9I2K
  SHALL be performed from the outside, to software components in an operating
  state, to look for security vulnerabilities (e.g. SQL injection, cross-site
  scripting).
* **[QC.Sec04]** Manual penetration testing MAY be part of the application security
  verification effort.
* **[QC.Sec05]** Security code reviews [9] for certain vulnerabilities SHOULD be done as part
  of the identification of potential security flaws in the code. Inputs SHOULD
  come from automated linters and manual penetration testing results.
* **[QC.Sec06]** World-writable files or directories MUST NOT be present in the product’s
  configuration or logging locations.
* **[QC.Sec07]** World-writable files SHOULD NOT be created while the service is in
  operation. Whenever they are required, the relevant files MUST be documented.
* **[QC.Sec08]** World-readable files MUST NOT contain passwords.
* **[QC.Sec09]** The services delivered SHALL adhere to any extra security policies or
  requirements set at the operational level.

### Code Review [QC.Rev]

Code review implies the informal, non-automated, peer, human-based revision of
any change in the source code. It appears as the last step in the change
management pipeline, once the candidate change has successfully passed over the
required set of change-based tests.

* **[QC.Rev01]** Code reviews MUST be done in the agreed peer review tool within the project,
  with the following RECOMMENDED functionality:
  * **[QC.Rev01.1]** Allows general and specific comments on the line or lines that need to
    be reviewed.
  * **[QC.Rev01.2]** Shows the results of the required change-based test executions.
  * **[QC.Rev01.3]** Allows to prevent merges of the candidate change whenever not all the
    required tests are successful.
  Exceptions to this rule cover the third-party or upstream contributions
  which MAY use the existing mechanisms or tools for code review provided by
  the target software project. This exception MUST only be allowed whenever
  the external revision lifecycle does not interfere with the project
  deadlines.
* **[QC.Rev02]** Code reviews MUST be open and collaborative, allowing external expert
  revisions.
* **[QC.Rev03]** Code reviews SHOULD be concise and use neutral language. The areas where the 
  reviewers MAY focus are:
  * **[QC.Rev03.1]** Message description: commit message is clear, self-explanatory and
    describes precisely the objectives being addressed.
  * **[QC.Rev03.2]** Goal or scope: change is needed and/or addresses/fixes the whole set of
    objectives.
  * **[QC.Rev03.3]** Code analysis: useless statements in the code, library or modules
    imported but never used or code style suggestions.
  * **[QC.Rev03.4]** Review of required tests: current battery of tests is sufficient for
    validation.
  * **[QC.Rev03.5]** Review of documentation: whether the change SHOULD bring along a
    corresponding update in the documentation.
* **[QC.Rev04]** Code reviews MUST be checked on change basis.
* **[QC.Rev05]** Code reviews SHOULD assess the inherent security risk of the changes,
  ensuring that the security model has not been downgraded or compromised by
  the changes.

### Automated Deployment [QC.Aud]

* **[QC.Aud01]** Production-ready code SHALL be deployed as a workable system with the minimal
  user or system administrator interaction leveraging software configuration
  management (SCM) tools.
* **[QC.Aud02]** A SCM module is treated as code.
  * **[QC.Aud02.1]** Version controlled, it SHOULD reside in a different repository than the
    source code to facilitate the distribution.
* **[QC.Aud03]** It is RECOMMENDED that all software components delivered by the same project
  agree on a common SCM tool.
  * **[QC.Aud03.1]** However, software products are not restricted to provide a unique
    solution for the automated deployment.
* **[QC.Aud04]** Any change affecting the application’s deployment or operation MUST be
  subsequently reflected in the relevant SCM modules.
* **[QC.Aud05]** Official repositories provided by the manufacturer SHOULD be used to host
  the SCM modules, thus augmenting the visibility and promote external
  collaboration.


## Glossary

__API__
: Application Programming Interface

__CLI__
: Command Line Interface

__DAST__
: Dynamic Application Security Testing

__EOSC__
: European Open Science Cloud

__OWASP__
: Open Web Application Security Project

__SAST__
: Static Application Security Testing

__SCM__
: Software Configuration Management

__SQA__
: Software Quality Assurance

__VCS__
: Version Control System


## References {.page_break_before}

<!-- Explicitly insert bibliography here -->
<div id="refs"></div>
