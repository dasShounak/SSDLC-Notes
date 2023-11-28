# SSDLC Revision Notes

## Table of Contents
- [Unit 1](#unit-1)
- [Unit 3](#unit-2)
- [Unit 3](#unit-3)
- [Unit 4](#unit-4)
- [Unit 5](#unit-5)

## Unit 1

### Software Development Models

- Waterfall Model
	- Sequential, plan-driven
	- Easy
	- Minimum customer involvement
	- Can't adapt to changes
	- Phases (RDITDM)
		- requirements
		- design
		- implementation
		- testing
		- deployment
		- maintenance
- Incremental
	- divides into small increments
	- delivered quickly
	- user feedback important
- Iterative
	- build small portions
	- release for feedback
	- easy to fix flaws
	- modular
- RAD
	- based on iterative and prototyping
	- little planning
		- Analysis and design
		- develop, demonstrate, refine
		- testing
		- deployment
- Spiral
	- Risk driven
	- loops
	- urgent and unclear projects
		- planning
		- risk identification
		- development and testing
		- analysis

### Agile

- swift and versatile
- based on iterative model
- break tasks into smaller increments
- well planned
- phases
	- requirements gathering
	- design
	- construction/iteration
	- testing
	- deployment
	- feedback
- models
	- Scrum - development by small teams
	- crystal
	- DSDM (dynamic software development method)
	- FDD (feature driven development)
	- lean software development
	- XP (extreme programming)

### Need for SSDLC

- High connectivity in the world leads to huge threat environment
- Attacker can access private and sensitive data or use compromised system to attack other users
- The cost-benefit ratio is defined by Clark and Davis (1995)


$$M_{b}+ P_{b}> O_{cp} + O_{cm}P_{a}P_{c}$$  
$M_{b}$ = Monetary benefit of attacker  
$P_b$ = Psychological benefit of attacker  
$O_{cp}$ = Cost of committing the crime  
$O_{cm}$ = Monetary costs of conviction (legal costs)  
$P_a$ = probability of getting arrested  
$P_c$ = probability of conviction for the attacker  

- Privacy is a way of *complying* with policy 
- Security is a way of *enforcing* the policy

### Critical Mass

- There must be enough knowledgeable people reviewing enough of the code often enough
- A critical mass of experienced and willing eyes makes all bugs shallow

### Proprietary Software Development Methods

- CMMI
	- **capability maturity model integration**
	- maturity level
		- foundation for *continuous process development*
	- lower level -> higher risk, lower quality
	- levels (IMDQO)
		- initial
		- managed
		- defined
		- quantitatively managed
		- optimizing
- TSP
	- **team software process**
	- team concepts in development
	- steps
		- establish goals
		- define team roles
		- assessing risks
		- producing team plan
- PSP
	- **personal software process**
	- helps in developing skills at a personal level
	- levels
		- PSP 0  - measurements,  coding standards
		- PSP 1 - time and scheduling
		- PSP 2 - personal quality management and code reviews
		- PSP 3- personal process evolution

## Unit 2

### Risk Management Framework (RMF)

- RMF - philosophy for software security
- Its a lifecycle
- Identifying and keeping track of risks
- Occurs in parallel with SDLC activities
- Not time consuming
	- Automation - large companies
	- Small teams - medium companies
	- Individual part-time task - small companies
- Threats - events that could cause harm potentially
- Vulnerability - weakness in IT systems
- Impact - measurement of how severe the harm could be
- Likelihood - measurement of risk factor 
- Predisposing conditions - factors that increase/decrease impact or likelihood
	- Risk = Threat x Vulnerability x impact/asset value
	- Level of Risk = Consequence x Likelihood
- Stages (UISDF)
	- understand business context
	- identify business and technical risks
	- synthesize and prioritize risks 
	- define risk mitigation strategy
	- fix and validate 
- risk metrics
	- risk likelihood
	- risk impact
	- risk severity
	- number of risks emerging and mitigated over time

### Stage 1: Understanding Business Goals

- business goals are neither obvious nor explicitly stated
- the analyst must extract and describe business goals, priorities, and circumstances 
- Business goals include but are not limited to increasing revenue, meeting *service-level agreements (SLAs)*, reducing development costs, and generating high *return on investment (ROI).* 
- Ask "Who cares?"

### Stage 2: Identify Business and Technical Risks

- **Business Risks:**
  - Threaten business goals with impacts like financial loss, brand damage, regulatory violations.
  - Severity expressed in financial terms (market share, cost).

- **Business Risk Identification:**
  - Clarifies and quantifies events impacting goals.
  - Foundation for technical methods in software risk mitigation.

- **Tying Technical Risks to Business Context:**
  - Essential for effective risk management.
  - Thorough identification and understanding are crucial.

- **Discovering and Describing Technical Risks:**
  - Central to RMF, involves situations counter to planned system design.
  - Examples: unexpected behavior, design violations.

- **Impacts of Technical Risks:**
  - Include system crashes, control avoidance, unauthorized data modification.

- **Technical Risk Identification Support:**
  - Supported by software security touchpoints.

### Stage 3: Synthesize and Prioritize Risks

- prioritization of risks leads directly to creation of value. 
- Answers the "Who cares?" question
- which business goals are the most important to the organization, which goals are immediately threatened
- Risk metrics
	- likelihood
	- impact
	- severity
	- number of risks emerging and mitigated over time

### Stage 4: Define Risk Mitigation Strategy

- **Security Challenge:**
  - Analysts find issues but lack clear solutions.
  - Mitigation strategy is essential for a robust risk analysis.

- **Fixing Complexity:**
  - Widespread among security consultants.
  - Designing resilience is harder than finding vulnerabilities.

- **Mitigation Strategy Focus:**
  - Develop cost-effective strategy post risk identification.
  - Considers cost, time, success likelihood, completeness, and impact.

- **Strategic Constraints:**
  - Aligned with business context.
  - Considers affordability, integration, and organizational understanding.
  - Emphasizes direct validation techniques.

- **Metrics in Mitigation:**
  - Financial metrics applied: cost takeout, ROI, method effectiveness, and risk coverage percentage.


### Stage 5: Carry out Fixes and Validate

- Problems must be rectified
- progress should be measured in terms of completeness against the risk
- validation provides confidence that the risks have been properly mitigated
- testing can be carried out


## Unit 3

### Architectural Risk Analysis

- identifies flaws in a software architecture
- determines risks to business information assets that result from those flaws
- Stages (RATCTF)
	- Requirements
	- Architecture and Design
	- Test plans
	- Codes
	- Test Results
	- Feedback
- Steps (AARR)
	- Asset Identification
	- Architectural Risk Analysis
		- Threats
		- Vulnerabilities
	- Risk Mitigation
	- Risk Management and Measurement
- Prototypical Risk Analysis
	- Learn
	- Discuss security issues
	- Determine probability of compromise
	- Impact analysis
	- Rank risks
	- Report findings
- Forest level view
	- building a consistent view of the target system
	- idea is to see the forest and not get lost in the trees
	- One-page overview or forest view - the big picture
		- UML diagrams

### Risk calculation

$ALE = SLE \times ARO$

ALE = Annual Loss Expectancy
SLE = Single Loss Expectancy
ARO = Annual Rate of Occurrence

## Unit 4

### Code Review with a Tool

- Debugging is at least twice as hard as programming
- If your code is as clever as you can possibly make it, then by definition you're not smart enough to debug it.
- All software projects are guaranteed to have one artifact in common—*source code.*
- large number of security problems are caused by simple bugs
- code review is about finding and fixing bugs.
- Using a tool makes sense because code review is boring, difficult, and tedious.
- Code review is critical for the following reasons:
	- no bugs in code
	- minimize having issues
	- new code adheres to guidelines
	- efficiency of new code
- cause of bugs
	- missing semicolons
	- most programming languages were not designed with security in mind
	- misuse of functions

### Static Analysis

- examine text of program statically
- manual auditing
	- can be time consuming
- tools are faster
- can be applied before program reaches a level of completion
- The earlier security risks are identified and managed in the software lifecycle, the better.

### Binary Analysis

- Source code analyzers are particularly useful when you're building software
- When no source code?
	- attackers really don't need source code to find vulnerabilities and develop exploits 
	- *disassemblers* and *decompilers* are tools that feature prominently in the attacker's toolkit.
	- binary analysis is important
- threat assessment and security assessment framework at a *binary level of code*
- **static application security testing (SAST)** is a technological toolset that can analyze various static codes, like binary code, byte code, and application source code while they are in a non-running state

### Tools from Researchland

| Tool       | Function                                                       |
| ---------- | -------------------------------------------------------------- |
| BOON       | Integer range analysis of C programs                           |
| CQual      | Taint analysis, format string vulnerabilities in C             |
| xg++       | Compiler extension, finding kernel vulnerabilities             |
| Eau Claire | Specification checking framework                               |
| MOPS       | Model-checking approach to look for temporal safety violations |
| Splint     | Lint in security


### Key Characteristics of a Tool

1. Designed for security
2. Support multiple tiers
3. Extensible
4. Can be used by security analysts as well as developers
5. Support existing development processes
6. Make sense to multiple stakeholders


## Unit 5

