![Philips Open Source Logo](assets/philips_open_source.png)

# Open Source at Philips

1. [Purpose](#purpose)
1. [Key Considerations](#considerations)
1. [Open Source Procedure](#process)
1. [Rules](#rules)
1. [Contact](#contact)
1. [Appendix 1: MIT license](#A1)
1. [Appendix 2: How to honor non-Philips third-party OSS components](#A2)
1. [Appendix 3: Why you must create a new repo](#A3)

<a name="purpose"></a>
## 1. Purpose
This document has been created by the Philips [Open Source Team](#contact) and describes open sourcing (publishing) a project.

Philips employees: please use the [internal version](https://gitlab.ta.philips.com/open-source/howto-open-source), which contains a few internal links.

<a name="considerations"></a>
## 2. Key Considerations
Open source is a decentralized process:
+ Not all contributions/use can be evaluated by formal bodies
+ Contributor has the main insights/knowledge on code that is contributed
+ **The contributor is responsible**

With help of the Open Source Team and the contributor's Department Head, it is the contributor's responsibility is to ensure that:
### 2.1 The contribution delivers value
It is hard to predict the impact of your contribution. One of the reasons we do Open Source is to find out what resonates with the community. Still, when preparing your contibution, do your homework. Is your contribution unique in some sense? Is it a new approach to solve a problem or does it make an existing solution more robust? The judgement is yours, but you should be able to answer these kind of questions. 

### 2.2 Nothing is published that might risk Philips’ competitive advantage
Take a considerate approach and reach out to Legal, Communications, and/or the [Open Source Team](#contact) for any ambiguous cases.

### 2.3 The contribution is of sufficient quality
Your contribution to Philips Open Source is not just *your thing*, but it also casts some light on the engineering culture at Philips and reflects on the Philips Brand. For this reason it is crucial that each contribution fulfils some basic hygiene factors. These hygene factors aim at making your contribution easier to understand to the contributors and encourage them to contribute. 

<a name="process"></a>
## 3. Open Source Procedure 
To publish your project on the Philips corporate GitHub account, please follow these steps:
1. Read all the [rules](#rules) below and make sure your project complies with them.
2. Email the Open Source Team about your project with the following information:
    + Project name and link
    + Do you plan to promote your project internally and externally, to build a community of users and contributors?
    + Does this project have any internal Philips dependencies? (If "Yes," stop here.)
    + Who is your target audience?
    + How many hours per week will you devote to maintaining and growing the project?
    + What does this project solve for potential users, and how is it different (better, faster, simpler) than existing solutions?
3. The Open Source Team will review your project and offer feedback and guidance to support your publication bid.
4. The Open Source Team might ask you to present your project, but in most cases will request information over email/instant message.
5. For your project to go live, you must receive approval from the Open Source Team (assessment of the [key considerations](#considerations)).
6. Upon receiving the Open Source Team's approval, you can push your project to the [Philips corporate GitHub account](https://github.com/philips-software).

The [Open Source Team](#contact) is there to support you in case of questions regarding your contribution. 


<a name="rules"></a>
## 4. Rules
The rules below serve as a basic quality assessment.
1. You MUST create a meaningful `README.md` ([template](templates/README.md)).
2. All projects MUST include a `MAINTAINERS.md` ([template](templates/MAINTAINERS.md)) file listing at least two active maintainers by name and contact email.
3. You MUST include a `CONTRIBUTING.md` ([template](https://github.com/nayafia/contributing-template)) guidelines file.
4. You MUST create a `LICENSE.md` file. Contact Legal for personal support on licensing.
5. You SHOULD semantically version project artifacts. You MUST tag all versions in GitHub with the exact version name: e.g., 0.1.0.
6. Your repositories MUST NOT, at any time, include Philips specifics such as credentials and private identifiers.
7. Your contribution MUST NOT, at any time, include anything that might risk Philips’ competitive advantage - see Section 2.2 above, nor should it negatively impact the Philips brand.
8. You MUST create an entirely new Git repository before pushing the project to GitHub. More info in [Appendix 1](#A1).

<a name="contact"></a>
## 5. Contact
### Philips Open Source Team
- [Marcin Czenko](https://github.com/marcinczenko)
- [Bart Golsteijn](https://github.com/bartgolsteijn/)
- [Ralph Holdorp](https://github.com/ralphholdorp)
- [Jeroen Knoops](https://github.com/jeroenknoops)
- [Arnold Niessen](https://github.com/ArnoldNiessen)
- [Niek Palm](https://github.com/npalm)

----

<a name="A1"></a>
### Appendix 1: Why you must create a new repo
“You MUST create an entirely new Git repository before pushing the project to GitHub.”

This rule is a trade-off. On the one hand, we lose information when creating a new git repository. On the other hand, keeping a long history in an existing repository is too-high risk; specifics like credentials could be published by mistake. Security comes first.
