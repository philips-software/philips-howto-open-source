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
1. [Appendix 4: Contributing to an existing open source project](#A4)

<a name="purpose"></a>
## 1. Purpose
This document has been created by the Philips [Open Source Team](#contact) and describes the process for open sourcing (publishing) a project.

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
This could include (but is not limited to):
+ Philips-specific projects: things tightly coupled to/dependent upon our systems
+ Domain knowledge
+ Customer data
+ Unique Selling Points (USPs)
+ Medical Claims
+ Trade secrets
+ Anything else that would risk our competitive advantage or could harm the Philips Brand

Take a considerate approach and reach out to Legal, Communications, and/or the [Open Source Team](#contact) for any ambiguous cases.

Anything that a Philips business or venture does not want to be published as Open Source, must not be published. 

### 2.3 The contribution is of sufficient quality
Your contribution to Philips Open Source is not just *your thing*, but it also casts some light on the engineering culture at Philips and reflects on the Philips Brand. For this reason it is crucial that each contribution fulfils some basic hygiene factors. These hygene factors aim at making your contribution easier to understand to the contributors and encourage them to contribute. In assessing the quality of your contribution we pay special attention to the elements that improve the clarity of your publication. We are less critical about technical content. E.g. if we recommed that your source code has automated tests, we do not judge what is the right level of testing or how you should test specific parts of your code. We assume that the contributor knows better in the end. The [rules](#rules) below form a basic quality assessment.

### 2.4 The contribution does not contain anything to which export control restrictions apply
E.g. AI tools and toolkits that we may be basing our contributions on come with export control restrictions that we may inherit, and some of the tools that we create may have ECO even if the project does not (dual use in AI/ML/DL). 

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
4. You MUST create a `LICENSE.md` file and state that the MIT license applies to all code owned by Philips within your contribution. (Please use the license text in [Appendix 1](#A1)). If you use third-party OSS, you MUST only use license-compatible projects/software. You MUST honor the original licenses used in those third-party projects in the license file (see [example](templates/LICENSE.md)). For more information and guidance, see [Appendix 2](#A2). Contact Legal for personal support on licensing.
5. You SHOULD semantically version project artifacts. You MUST tag all versions in GitHub with the exact version name: e.g., 0.1.0.
6. Your repositories MUST NOT, at any time, include Philips specifics such as credentials and private identifiers.
7. Your contribution MUST NOT, at any time, include anything that might risk Philips’ competitive advantage - see Section 2.2 above, nor should it negatively impact the Philips brand.
8. You MUST create an entirely new Git repository before pushing the project to GitHub. More info in [Appendix 3](#A3).

<a name="contact"></a>
## 5. Contact
### Philips Open Source Team
- [Ralph Holdorp](mailto:ralph.holdorp@philips.com)
- [Bart Golsteijn](mailto:bart.golsteijn@philips.com)
- [Marcin Czenko](mailto:marcin.czenko@philips.com)

Please contact the Open Source Team if you would like to become a member.

### Owner
- [Ralph Holdorp](mailto:ralph.holdorp@philips.com)


----
<a name="A1"></a>
### Appendix 1: MIT License 
Replace the [yyyy] field with the year that you created the project, and do not update it. Do not provide multiple years.

```
The MIT License (MIT) Copyright © [yyyy] Koninklijke Philips N.V, https://www.philips.com

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

<a name="A2"></a>
### Appendix 2: How to honor non-Philips/third-party OSS components
Copyleft: Copyleft is a legal obligation that Philips must fulfill when you modify and/or distribute and/or make third party material publicly available (so-called “copyleft trigger”). 

Examples: changing the program code, uploading to public GitHub, sending it to someone else from another company. Copyleft may oblige Philips to license its modifications also under the license whose copyleft was triggered. In legal terms, “modification” can be interpreted very broadly, e.g. whole libraries or code that you added (so-called “scope of copyleft”).
 
For Modification + Internal and/or Publishing, do not use reciprocal licenses that trigger the copyleft already during internal modification, e.g. RPL or APSL 2.1, AGPLv3.
 
For Modification + Publishing:
+ See above (RPL, ASPL 2.1, AGPLv3, etc.).
+ Do not use licenses with strict copyleft, e.g. GPLv2, GLPLv3, unless you have clearance from Legal.
+ If you use licenses with limited copyleft (e.g. LGPLv2.1, LGPLv3, MPLv2, CPL), please make sure you can fulfill their specific requirements to restrict the copyleft from taking over Philips' or other third-party’s code. → reach out to Legal.

License Template for Multi-Licensed Projects without Copyleft

```
This {name} Project is in general licensed under the following MIT license except the files named underneath (see corresponding notice files below) 

    (Insert Philips MIT from Appendix 1 above)

Notice file for (path)/(other file) 

    (Insert license text & copyright notice from the original file here)

Notice file for (path)/(other file) 

    (Insert license text & copyright notice from the original file here)

 (...)
```

<a name="A3"></a>
### Appendix 3: Why you must create a new repo
“You MUST create an entirely new Git repository before pushing the project to GitHub.”

This rule is a trade-off. On the one hand, we lose information when creating a new git repository. On the other hand, keeping a long history in an existing repository is too-high risk; specifics like credentials could be published by mistake. Security comes first.

<a name="A4"></a>
### Appendix 4: Contributing to an existing open source project
More information about contributing to an open source project can be found [here](contributing-to-open-source.md).
