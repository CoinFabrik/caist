# Collaborative Artificial Intelligence Security Tool (CAIST)

## Summary of your project
In this project we want to build a tool to assist in the detection of vulnerabilities in smart contracts. This tool will leverage powerful artificial intelligence constructs like Open AI’s LLMs, and our knowledge and experience, in manual security audits. 

Existing smart contract security tools do not suffice: even when the distributed apps are developed by very professional teams (e.g., check https://rekt.news/leaderboard/ ). Tools used to find bugs in Solidity/Eetherem smart contracts -for example- may require extensive setup, they generate a good deal of false positives for which developers need to invest serious time to discard. In reality, no research like this has been tried or published. If successful, it will provide a breakthrough improving security overall and spanning more research. We believe that there is an exponential and untapped growth of LLMs that may well solve security problems. Hence, our aim is to combine a great deal of experience in Security Research with LLMs power to build this tool.
Building Collaborative Artificial Intelligence Security Tool (CAIST), will combine automatic, human, and AI analysis techniques. Our goal is to allow developers, security auditors, and QA specialists to iterate in a bug-finding process with the intervention of multiple artificial intelligence techniques. Human-machine iteration makes the search for security issues to be reinforced positively.

Using AI clustering will focus on identification of potential issues and implement a semantic query language to facilitate computer-human interactions. In order to facilitate bug-finding, CAIST starts with a classification phase where Solidity smart contracts are included in categories (e.g. AMMs) and subcategories, next elicits questions (and helps to answer them) particularly to the smart contracts (sub)categories, and assists in either confirming or rejecting a security issue.

We divided the problem into subproblems that we will solve according to the accompanying roadmap. The development of CAIST is outlined in a five milestone project which are:
- Milestone 1: Component classification POC tool
- Milestone 2: Classification of vulnerable smart contracts
- Milestone 3: Manual querying for vulnerability detection
- Milestone 4: POC tool for automatic LLM querying for vulnerability detection
- Milestone 5: Development of an integrated platform

Current proposal concentrates on the first milestone.

### About CoinFabrik
CoinFabrik is a pioneering research, development, and security auditing company with a distinct focus on Web3 technologies. Established in 2014, our extensive portfolio comprises over 200 projects related to Web3, spanning the globe. Ranging from dynamic startups to industry giants, our expertise extends across a spectrum of cutting-edge technologies. Including but not limited to Bitcoin, Ethereum, Polygon, Solana, Polkadot, Stacks, NEAR, and Algorand, operating seamlessly across various layers of Web3. At CoinFabrik, we embrace technological agnosticism, constantly seeking optimal solutions to meet and exceed the unique requirements of our clients or initiatives. Our commitment lies in delivering excellence and innovation as we navigate the ever-evolving landscape of Web3 technologies.

Our team has an academic background in computer science and mathematics, with work experience focused on cybersecurity and software development, including academic publications, patents turned into products, and conference presentations.

In Coinfabrik we have an audit service as one of our offerings. With it, we ensure submitted code or smart contract is transparent, tamper-proof and free of vulnerabilities before it is deployed. Smart contracts allow for secure execution of agreements between multiple parties using a computer program that operates on a blockchain network. The smart contract automatically performs the agreed-upon actions once deployed. Over the years, we have +200 audits so far.

As part of our structure, we have a R+D area which explores and creates new technologies, products, and services through systematic investigation and experimentation. Activities include basic research, applied research, and development of new products or processes. Successful R&D outcomes can lead to increased efficiency, cost savings, and revenue growth. We can mention some applications of this service:

- Security tools for identification of bugs and vulnerabilities
- Secure authentication platforms
- Authentication tools
- Access control systems
- Data and identity privacy  
- Secure voting systems
- Web3 Sysadmin services
- Tokenization of assets
- Blockchain R&D and support
- Decentralized solution development

### Our Recent Related Work
During 2023, we researched clustering. This proof of concept aims to classify Solidity smart contracts unsupervised, aiming to create a vulnerability detection tool. Smart contracts are grouped into clusters based on functionality, providing a targeted vulnerability detection approach. Repositories from Github (2017-2023, >20 stars) were used, and main contracts were parsed for information. The initial approach involved listing function names and assessing their similarity. Clustering techniques, including DBSCAN, were applied to principal components for noise reduction, and contract networking via functions was studied. Promising outcomes revealed clusters such as DEX/DeFi platforms, Yield Farming & Staking, Governance, ERC Standards, Ownership Management. The research focuses on refining data processing and examining the best similarity measure and vector representation for the problem.

We have an ongoing collaboration on knowledge transfer and open-source projects with the Universidad de Buenos Aires in the context of MEGA-ACE project, funded by the Algorand Foundation, which aims to build a mobility network of researchers and students which allows the project to target research and implementation efforts to problems informed by the needs of societies in all five continents. Among other participating universities are Purdue University - USA, Cornell - USA, UCLA - USA; Bar-Ilan - Israel, Reichman University - Israel, Ecole Polytechnique - France, Universidad Nacional Autonoma de Mexico - Mexico, etc.

Throughout 2022 and early 2023, we collaborated with the Laboratory on Foundations and Tools for Software Engineering (LaFHIS) at the University of Buenos Aires to establish analysis techniques and tools for detecting vulnerabilities in code, as well as to create an initial list of vulnerability classes for smart contracts and code examples. We started this collaboration with a grant from NEAR Foundation in 2022, where we focused on reviewing available tools applicable for detecting vulnerabilities in Rust. This research was followed in 2023 by a series of grants financed by Web3 Foundation and Aleph Zero Ecosystem Grants, that led to the release of our vulnerability detector for smart contracts Scout.

We believe that, by working on a thorough classification of smart contract vulnerabilities, we can leverage LLM as a powerful technique for vulnerability detection. This would be a new application in the context of vulnerabilities for smart contracts in Solidity, as well as Rust based blockchains.

## Project proposal URL
- Public repo: https://github.com/CoinFabrik/caist
- CAIST page: https://www.coinfabrik.com/collaborative-artificial-intelligence-security-tool-caist/

## Proposed completion date
Milestone 1 has a duration of 8 weeks.

## OpenAI will provide funding and/or API credits for the research. How much of either will you need?
Milestone 1 funds are USD 48,000.

## Please describe how the funds will be used for your project, and outline how you arrived at the value 

### Milestone 1: Component classification POC tool
#### Milestone 1.1: Process to collect initial set of smart contracts
- Purpose: Design a semi-automated process for nurturing a database of smart contracts. Populate database with 5,000+ smart contracts.
- Duration: 1 week.
- Funds: USD 6,000.
#### Milestone 1.2: Execution of clustering algorithms
- Purpose: Run clustering algorithms based on functionalities included in smart contracts, and find out what is their clustering capability.
- Duration: 3 weeks.
- Funds: USD 18,000.
#### Milestone 1.3: Create taxonomy of smart contract classes
- Purpose: Deduce at least one taxonomy of smart contract classes.
- Duration: 3 weeks.
- Funds: USD 18,000.
#### Milestone 1.4: Development of component classification POC Tool
- Purpose: Produce a proof of concept smart contract clustering algorithm which works with reasonable POC-precision.
- Duration: 1 week.
- Funds: USD 6,000.
### Assigned Team
Team will be composed by:
- 1 Project Manager (partial dedication)
- 1 Technical Leader (partial dedication)
- 1 Researcher (full dedication)
- 2 Developers (full dedication)

## Please provide a roadmap for the project on a one year time horizon

- Milestone 2: Classification of vulnerable smart contracts
-- Collect 200+ audited smart contacts. Research succinct vulnerability classification based on audits.
-- Tag the smart contracts according to the vulnerabilities they are reported to have.

- Milestone 3: Manual querying for vulnerability detection
-- Define a comprehensive list of human questions and workflow security auditors follow in the quest for understanding the codebase, and looking and finding vulnerabilities.
-- Using the control group, we want to build for each vulnerability class, a set of questions which, when answered, allow us to detect an instance of this vulnerability.

- Milestone 4: POC tool for automatic LLM querying for vulnerability detection
-- Prompt engineering.
-- Manually experiment with query tree. Record test results and validate functionality.
-- tool implementation

- Milestone 5: Development of an integrated platform
-- Develop a comprehensive integrated platform including GUI and integration with frameworks and repository hostings.
-- Publish tool repository and technical documentation.
