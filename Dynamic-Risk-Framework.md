<!-- Output copied to clipboard! -->

<!-----

You have some errors, warnings, or alerts. If you are using reckless mode, turn it off to see inline alerts.
* ERRORs: 0
* WARNINGs: 0
* ALERTS: 1

Conversion time: 2.775 seconds.


Using this Markdown file:

1. Paste this output into your source file.
2. See the notes and action items below regarding this conversion run.
3. Check the rendered output (headings, lists, code blocks, tables) for proper
   formatting and use a linkchecker before you publish this page.

Conversion notes:

* Docs to Markdown version 1.0β33
* Mon Dec 12 2022 06:41:56 GMT-0800 (PST)
* Source doc: Stablecoin Scoring Methodology
* Tables are currently converted to HTML tables.
* This document has images: check for >>>>>  gd2md-html alert:  inline image link in generated source and store images to your server. NOTE: Images in exported zip file from Google Docs may not appear in  the same order as they do in your doc. Please check the images!


WARNING:
You have 11 H1 headings. You may want to use the "H1 -> H2" option to demote all headings by one level.

----->


<p style="color: red; font-weight: bold">>>>>>  gd2md-html alert:  ERRORs: 0; WARNINGs: 1; ALERTS: 1.</p>
<ul style="color: red; font-weight: bold"><li>See top comment block for details on ERRORs and WARNINGs. <li>In the converted Markdown or HTML, search for inline alerts that start with >>>>>  gd2md-html alert:  for specific instances that need correction.</ul>

<p style="color: red; font-weight: bold">Links to alert messages:</p><a href="#gdcalert1">alert1</a>

<p style="color: red; font-weight: bold">>>>>> PLEASE check and correct alert issues and delete this message and the inline alerts.<hr></p>



# A Dynamic Stablecoin Evaluation Framework

**Date**: 		December 13th, 2022

**Authors**: 	Lavi & Dabar90


## Abstract


## Introduction

Stablecoins are cryptocurrencies that are pegged to a stable asset, such as the US dollar, to reduce volatility and provide a stable store of value. However, stablecoins have faced several challenges and criticisms. One of the main issues is that the peg to the underlying asset is not always reliable. Another problem is that some of the most prominent stablecoins are issued by private companies. Most decentralized stablecoins on the other hand still lack wider adaption. Besides these fundamental issues, there are many other risk that come with financial primitives in web3.

Despite these challenges, the use of stablecoins is growing. In fact, stablecoins are one of the most important innovations in DeFi, with one of the highest addressable markets of all use cases. Thus, the number of projects issuing stablecoins is also growing rapidly. 

As of today, very little has been done in terms of identifying, articulating, or measuring the risks related to those projects. It’s very difficult for everyday users to accentuate the quality of today’s stablecoin landscape. With this whitepaper, we aim to create a foundation for defining an evaluation framework for stablecoins. Primarily to facilitate identifying and measuring all relevant components that can introduce certain risks to these protocols. In essence, this documentation will provide a detailed explanation of how stablecoins can be evaluated.

The objectives of this whitepaper are as follows:



1. Create a holistic overview of all relevant aspects of stablecoin projects 
2. Enable comparison between stablecoins by setting a standard
3. Facilitate risk assessments and enable real-time health metrics


## An Approach to Creating a Risk Framework

To achieve these objectives, we first need to create a holistic overview of all relevant aspects of stablecoin projects. In other words, what components are required for a stablecoin project to become viable, and in an ideal scenario, become a sustainably viable alternative to fiat money. We largely base the core pillars around the stablecoin trilemma. In addition, we apply standard fundamental analysis concepts that help identify the quality and risks of stablecoin protocols.

In the second step, we need to make all relevant components measurable. For this, we fully rely on publicly available metrics. Basing the evaluation framework on fundamental key metrics introduces an objective foundation to calculate the scores. In return, we forgo certain equally important dimensions (e.g. the team or community). These are more complicated to measure and thus more difficult to compare objectively. Hence, we postpone coverage of these aspects to a later version.

Still, it is tricky to fully eliminate subjective assumptions. Despite only using public key metrics, subjectivity comes into play when weighing the scores. Essentially the final score of a project is decided by how well it scored per category, in combination with how much each category contributes to the overall score. In order for this system to be representative, and as close to the truth as possible, we have to set a clear perspective. While trying to strike the right balance between all components, we essentially lean more toward the perspective of stablecoin users.

Hence, the main focus is on existing or potential risks for stablecoin holders. The framework is not targeted toward governance token holders, or investors of the entity issuing the stablecoin. Therefore, we first and foremost pay attention to components that, from our point of view, pose a risk to end users of the stablecoin. For example, we assume that decentralization is a important, and that centralization can pose a significant risk, hence it is slightly higher weighted than scalability. But we will explain the weighting in more detail below.


## Evaluation Framework Overview

The review standard will assess stablecoins based on six main categories. The first three points are based on the stablecoin trilemma. Those categories aim to evaluate how well a project solves each of the three problems described in the stablecoin trilemma (see next section).

The fourth category is used to provide an in-depth understanding of the collateral that is backing the stablecoin. The underlying collateral is a very important piece of the puzzle. It touches all three aspects of the stablecoin trilemma. For instance, when using centrally issued currencies as backing, it influences the decentralization ratio. Relying on collateral with low availability can impact the scalability of the project. And when using highly volatile or low-quality tokens to back the stablecoin, it can affect the price stability.

The last category aims to provide insights into the technical quality of the protocol. As with all projects that rely on smart contracts, code quality and technical sophistication are very important risk vectors. Most hacks or exploits happen due to technical issues and unheeding security.

As mentioned above, this risk framework aims to be as objective as possible. Thus, we start with a rather lean version. We forgo the inclusion of other relevant dimensions to prove the viability of this basic version. Other fundamental aspects such as team, governance, partnerships, integrations, or regulatory risks can be added in later versions. Furthermore, we also aim to introduce the scoring of yield-bearing synthetic stablecoin representations, such as aDAI or cUSDC for instance. This will require the rather extensive evaluation of the lending protocol (e.g. Aave and Compound), which is deferred to a later stage of this project.

For readers already familiar with the stablecoin trilemma, we recommend skipping the next section and moving directly to the Scoring Overview.


## The Stablecoin Trilemma

The stablecoin trilemma describes the three problems that a stablecoin needs to solve, in order for it become a viable alternative to fiat money. The three problems are price stability, decentralization, and scalability (capital efficiency).



<p id="gdcalert1" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image1.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert2">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image1.png "image_tooltip")


(Source: [Twitter](https://twitter.com/chainlinkgod/status/1528954630813667328))

As of today, there is no stablecoin that embodies all three simultaneously at scale. Typically, stablecoin projects neglect one component in favor of the other two. For instance, USDC and USDT are 100% custodial and centralized. The collateral backing these stables is stored off-chain and custodied by centralized entities. This poses the risk of a single point of failure. Moreover, this setup is not censorship-resistant. Circle has already blacklisted certain addresses from using their stablecoin USDC.

MakerDAO’s DAI, for instance, was initially targeted to be a fully decentralized stablecoin. This objective was relinquished over the past years, as the community had difficulties scaling the project when only accepting ETH or WBTC as collateral. To solve this, they started to accept centralized USDC as backing. As a result, DAI is actually more like wUSDC, with over 60% of DAI being backed by USDC.

There is also the tragic example of Terra and UST. This project scaled very fast and it was somewhat decentralized. But to achieve this, the project applied a reflexive backing system, with LUNA as the only collateral. LUNA was minted or burned, depending on the demand for UST. Essentially, this led to a deathspiral event, when UST depegged and more LUNA had to minted than the market was able to absorb.

In conclusion, we found that this trilemma provides a suitedable foundation to create a review framework. It’s a fair compromise to base the evaluation on, as all stablecoin projects have to face these three issues in their initial design. Of course, there are more issues and risk vectors in the actual implementation, hence we will augment the scoring system with additional categories.


## Stablecoin Classification

To facilitate the differentiation between stablecoin projects, we use a classification system. This will provide high-level separation including subcategories. In our framework, we are going to use the following four stablecoins categories.



1. **Custodial Stablecoins**

    These are stablecoins where they assets are stored off-chain. Typically one centralized entity has custody of the collateral assets (examples: USDT, USDC).

2. **Non-custodial Stablecoins**

    This category includes all stablecoin protocols that have their collateral on-chain. This is typically referred to as non-custodial, meaning that the collateral is held by smart contracts (examples: DAI, LUSD, sUSD).

3. **Algorithmic Stablecoins**

    This category refers to fully algorithmic “stablecoins” that don’t require collateral-backing. Some see this as the holy grail of stablecoins. However, the quotationmarks hint to the fact that none of these projects have achieved price stability so far (examples: AMPL, ESD)

4. **Hybrid Stablecoins**

    This last category encompasses projects that apply a mix of algorithmic and collateral-backed methods to create a stable asset (examples: FRAX).


The next tiers to differentiate stablecoin projects take into consideration the collateralization ratio, the collateral type, and finally their issuer type. At the end of this document is a full overview of the categoriaztion including some examples.


## Stablecoin Evaluation Framework Description

This final section will provide an in-depth description of the evaluation framework designed to measure the quality and risks of stablecoin projects. Initially, the review will consist of five main categories, which will be described in more detail below.


### Decentralization Score




# **Stablecoin Evaluation Framework**


# **1. Overview **

The overview section should provide a high-level introduction of the project. This helps to prepare the reader for what type of project the report is about. A good approach is to summarise the key activities of the protocol, and summarizing the findings of each section at the end.


```
Project Description:
Background story (when was it founded, by whom, specific intentions, etc.)
Purpose of the protocol
How does the protocol differentiate itself from its competitors, where is it similar
Any other important information that doesn't fit into any sections below
```





# **Scorecard**


<table>
  <tr>
   <td><strong>1</strong>
   </td>
   <td colspan="2" ><strong>Decentralisation</strong>
   </td>
  </tr>
  <tr>
   <td>1.1
   </td>
   <td>Decentralized Issuer/Governance
   </td>
   <td>X / 50
   </td>
  </tr>
  <tr>
   <td>1.2
   </td>
   <td>Governance Impact/Mutability
   </td>
   <td>X / 25
   </td>
  </tr>
  <tr>
   <td>1.3
   </td>
   <td>Distribution Score
   </td>
   <td>X / 25
   </td>
  </tr>
  <tr>
   <td>1.4
   </td>
   <td>Collateral Decentralization Ratio
   </td>
   <td>X / 50
   </td>
  </tr>
  <tr>
   <td colspan="2" ><strong>Total Decentralization Score</strong>
   </td>
   <td><strong>X / 150</strong>
   </td>
  </tr>
</table>



<table>
  <tr>
   <td><strong>2</strong>
   </td>
   <td colspan="2" ><strong>Usage & Adoption</strong>
   </td>
  </tr>
  <tr>
   <td>2.1
   </td>
   <td>Stablecoin Market Cap and Market Share
   </td>
   <td>X / 25
   </td>
  </tr>
  <tr>
   <td>2.2
   </td>
   <td>Circulating and Free Float Supply Ratio
   </td>
   <td>X / 25
   </td>
  </tr>
  <tr>
   <td>2.3
   </td>
   <td>Growth Rate
   </td>
   <td>X / 25
   </td>
  </tr>
  <tr>
   <td>2.4
   </td>
   <td>Average Daily Transactions
   </td>
   <td>X / 25
   </td>
  </tr>
  <tr>
   <td>2.5
   </td>
   <td>Transaction Growth
   </td>
   <td>X / 25
   </td>
  </tr>
  <tr>
   <td>2.6
   </td>
   <td>Number of Token holders
   </td>
   <td>X / 25
   </td>
  </tr>
  <tr>
   <td colspan="2" ><strong>Total Adoption Score</strong>
   </td>
   <td><strong>X / 150</strong>
   </td>
  </tr>
</table>



<table>
  <tr>
   <td><strong>3</strong>
   </td>
   <td colspan="2" ><strong>Price Stability</strong>
   </td>
  </tr>
  <tr>
   <td>3.1
   </td>
   <td>Price (off-peg) deviation % - over 7d, 30d, 90d and 180d
   </td>
   <td>X / 25
   </td>
  </tr>
  <tr>
   <td>3.2
   </td>
   <td>Price (off-peg) deviation % on historical “black swan” events 
   </td>
   <td>X / 25
   </td>
  </tr>
  <tr>
   <td>3.3
   </td>
   <td>Days in operation
   </td>
   <td>X / 25
   </td>
  </tr>
  <tr>
   <td>3.4
   </td>
   <td>Issuance and redemption mechanisms
   </td>
   <td>X / 25
   </td>
  </tr>
  <tr>
   <td>3.5
   </td>
   <td>Protocol/DAO/Company controlled stability mechanisms
   </td>
   <td>X / 25
   </td>
  </tr>
  <tr>
   <td>3.6
   </td>
   <td>Open market stability mechanisms
   </td>
   <td>X / 25
   </td>
  </tr>
  <tr>
   <td colspan="2" ><strong>Total Price Stability Score</strong>
   </td>
   <td><strong>X / 150</strong>
   </td>
  </tr>
</table>



<table>
  <tr>
   <td><strong>4</strong>
   </td>
   <td colspan="2" ><strong>Collateral Quality</strong>
   </td>
  </tr>
  <tr>
   <td>4.1
   </td>
   <td>Collateral structure (diversification level)
   </td>
   <td>X / 25
   </td>
  </tr>
  <tr>
   <td>4.2
   </td>
   <td>Capital efficiency (average CR in %) -
   </td>
   <td>X / 25
   </td>
  </tr>
  <tr>
   <td>4.3
   </td>
   <td>Collateral volatility
   </td>
   <td>X / 25
   </td>
  </tr>
  <tr>
   <td>4.4
   </td>
   <td>Collateral liquidity
   </td>
   <td>X / 25
   </td>
  </tr>
  <tr>
   <td>4.5
   </td>
   <td>Protocol/DAO/Company controlled stability mechanisms
   </td>
   <td>X / 25
   </td>
  </tr>
  <tr>
   <td>4.6
   </td>
   <td>Open market stability mechanisms
   </td>
   <td>X / 25
   </td>
  </tr>
  <tr>
   <td colspan="2" ><strong>Total Collateral Quality Score</strong>
   </td>
   <td><strong>X / 150</strong>
   </td>
  </tr>
</table>



<table>
  <tr>
   <td><strong>5</strong>
   </td>
   <td colspan="2" ><strong>Technical Security</strong>
   </td>
  </tr>
  <tr>
   <td>4.1
   </td>
   <td>Smart contract audits and bug bounty score
   </td>
   <td>X / 40
   </td>
  </tr>
  <tr>
   <td>4.2
   </td>
   <td>Smart contract architecture and complexity
   </td>
   <td>X / 40
   </td>
  </tr>
  <tr>
   <td>4.3
   </td>
   <td>Composability risks
   </td>
   <td>X / 35
   </td>
  </tr>
  <tr>
   <td>4.4
   </td>
   <td>Oracle risk
   </td>
   <td>X / 35
   </td>
  </tr>
  <tr>
   <td>4.5
   </td>
   <td>Penalty for hacks or exploits
   </td>
   <td>- X
   </td>
  </tr>
  <tr>
   <td colspan="2" ><strong>Total Technical Security Score</strong>
   </td>
   <td><strong>X / 150</strong>
   </td>
  </tr>
  <tr>
   <td colspan="2" ><strong>TOTAL SCORE</strong>
   </td>
   <td><strong>X / 800</strong>
   </td>
  </tr>
</table>






1. **Decentralization - 150 pts**

This first section aims to capture a stablecoins progress toward decentralization. Typically a project starts rather centralized, with the founding team having strong influence and impact. However, as projects mature, dependency on the team and other centralized partys should diminish further. Immutability of core smart contracts can also reduce reliance and thus, reduce risks of harmful changes.

**1.1 Decentralized Governance (50 pts)**


## Distributed governance allows token holders and community members to participate in the governance of open finance protocols. This section tries to identify whether a stablecoin’s governance system is sufficiently decentralized. To answer this, the question to be asked is: “can one entity or a small group, exert significant influence over the stablecoin or the protocol? This can be either via exclusive access rights to core functionalities (e.g. smart contracts) or high concentration of voting power.


## This first section is only relevant for non-custodial protocols. Fiat-backed stables with off-chain collateral will get 0 points.


## ** \
Answer:** \
 \
**Score: **


<table>
  <tr>
   <td><strong>Score</strong>
   </td>
   <td><strong>Description</strong>
   </td>
  </tr>
  <tr>
   <td>50
   </td>
   <td>Voting power is substantially decentralized, there is a large and active community, no central party or small group has majority voting power.
   </td>
  </tr>
  <tr>
   <td>40
   </td>
   <td>Voting power is fairly decentralized, there is an active community, no central party has majority voting power.
   </td>
  </tr>
  <tr>
   <td>30
   </td>
   <td>Voting power is somewhat decentralized or somewhat concentrated around a few addresses. Those are well-known and trusted community members.
   </td>
  </tr>
  <tr>
   <td>20
   </td>
   <td>Governance is rather centralized. Community can take influence, but voting power is in the hands of a few.
   </td>
  </tr>
  <tr>
   <td>10
   </td>
   <td>Governance is more or less centralized. The team makes all decisions.
   </td>
  </tr>
  <tr>
   <td>0
   </td>
   <td>The stablecoin is fully controlled by a centralized entity (no governance).
   </td>
  </tr>
</table>


**1.2 Governance Impact / Mutability (25 pts)**


## The second aspect to consider with regards to governance, is to understand how far reaching its impact can be. While governance can be beneficial to steer a project, stablecoins should not form an over-reliance on human/community intervention. Meaning that the protocol should limit the mutability of its core functionalities (specifically smart contracts) to only necessary parameters. Hence, to what extent are governance capabilities limited to necessary parameters only? Are there centralized components with significant access rights that can impact the protocol?** \
**


## **Answer:** \
 \
**Score: **


<table>
  <tr>
   <td><strong>Score</strong>
   </td>
   <td><strong>Description</strong>
   </td>
  </tr>
  <tr>
   <td>25
   </td>
   <td>Governance impact is limited to the necessary parameters. What should be immutable cannot be impacted. The change process is very robust (on-chain governance).
   </td>
  </tr>
  <tr>
   <td>20
   </td>
   <td>Governance has the right influence over core processes. Some contracts/parameters are immutable. The governance process is robust (on-chain).
   </td>
  </tr>
  <tr>
   <td>15
   </td>
   <td>Governance has far reaching powers and can change everything related to the protocols core contracts, operations, tokenomics, funding. Some (crucial) access controls are still centralized.
   </td>
  </tr>
  <tr>
   <td>10
   </td>
   <td>Governance only functions as a signal. The team has full access to core functionalities. But the team is trusted/well-known (they have good reputation).
   </td>
  </tr>
  <tr>
   <td>5
   </td>
   <td>The team has full access to all core functionalities. The team is public and trusted.
   </td>
  </tr>
  <tr>
   <td>0
   </td>
   <td>The team has full access to all core functionalities. The team is anon.
   </td>
  </tr>
</table>


**1.3 Supply Distribution (25 pts)**


## The supply distribution can help to better understand usage of a stablecoin. If there is a high supply concentration, this typically hints that the coin is mostly used by a few large holders. And not well established for retail use cases. To measure the distribution, the total number of addresses, that together hold 80% or more of the total supply, is measured.


## ** \
Answer:** \
 \
**Score: **


<table>
  <tr>
   <td><strong>Score</strong>
   </td>
   <td><strong>Description</strong>
   </td>
  </tr>
  <tr>
   <td>25
   </td>
   <td>80% of total supply is held by 1500 or more adresses
   </td>
  </tr>
  <tr>
   <td>20
   </td>
   <td>80% of total supply is held by 750 or more adresses
   </td>
  </tr>
  <tr>
   <td>15
   </td>
   <td>80% of total supply is held by 250 or more adresses
   </td>
  </tr>
  <tr>
   <td>10
   </td>
   <td>80% of total supply is held by 100 or more adresses
   </td>
  </tr>
  <tr>
   <td>5
   </td>
   <td>80% of total supply is held by less than 50 adresses
   </td>
  </tr>
  <tr>
   <td>0
   </td>
   <td>80% of total supply is held by less than 10 adresses
   </td>
  </tr>
</table>


**1.4 Collateral Decentralization Ratio (50 pts)**


## The entity issuing a stablecoin might be decentralized, censorship resistant, and fully immutable. However, there is little value in that when the collateral that is backing its stablecoin is subject to significant centralized control.


## The collateral decentralization ratio (CDR) measures the centralization risk of collateral tokens. Collateral with excessive off-chain risk (e.g. fiat-backed stables or custodial assets such as gold/oil etc) are considered to be 0% decentralized. ETH and BTC, as well as certain reward tokens such as AAVE or CRV for instance, are counted as 100% decentralized.


## The question that needs to be answered, is whether the collateral is subject to a centralized authority, and whether it has the potential to blacklist or otherwise limit usage, and thus change its viability as collateral.


## ** \
Answer:** \
 \
**Score: **


<table>
  <tr>
   <td><strong>Score</strong>
   </td>
   <td><strong>Description</strong>
   </td>
  </tr>
  <tr>
   <td>50
   </td>
   <td>CDR = 100% (e.g. collateral is 100% ETH)
   </td>
  </tr>
  <tr>
   <td>40
   </td>
   <td>CDR = 80% (e.g. collateral is 80% ETH & 20% USDC) 
   </td>
  </tr>
  <tr>
   <td>30
   </td>
   <td>CDR = 60% (e.g. collateral is 60% ETH & 40% USDT)
   </td>
  </tr>
  <tr>
   <td>20
   </td>
   <td>CDR = 40% (e.g. collateral is 40% ETH & 60% WBTC)
   </td>
  </tr>
  <tr>
   <td>10
   </td>
   <td>CDR = 20% (e.g. collateral is 20% ETH, 40% USDC & 40% USDT)
   </td>
  </tr>
  <tr>
   <td>0
   </td>
   <td>CDR = 0% (e.g. collateral is 100% USDC)
   </td>
  </tr>
</table>





# **2. Usage and Adoption (150 pts)**


## This section aims to evaluate a stablecoins adoption rate and general acceptance as method of payment.

**2.1 Adoption - Market Capitalization & Market Share (25 pts)**


## Market capitalization refers to the total value of the stablecoin. It is easily calculated by multiplying its value per unit (usually 1 USD) with its circulating supply. In addition, the market-share is used to quantify a stablecoins rank, when compared with its peers and competitors.


## ** \
Answer: ** \
 \
**Score: **


<table>
  <tr>
   <td><strong>Score</strong>
   </td>
   <td><strong>Description</strong>
   </td>
  </tr>
  <tr>
   <td>25
   </td>
   <td>Market Leader = Highest market cap and/or highest market share
   </td>
  </tr>
  <tr>
   <td>20
   </td>
   <td>Strong Competitor = 2nd or 3rd highest market cap and market share
   </td>
  </tr>
  <tr>
   <td>15
   </td>
   <td>Established Market Participant = ranking 4-8 in terms of market cap and share
   </td>
  </tr>
  <tr>
   <td>10
   </td>
   <td>New Entrant/Weak Competitor = ranking 9-20 market cap and share
   </td>
  </tr>
  <tr>
   <td>5
   </td>
   <td>Functional but not established = ranking 21 and lower
   </td>
  </tr>
  <tr>
   <td>0
   </td>
   <td>Fake, scam, or otherwise not-usable
   </td>
  </tr>
</table>


**2.2 Adoption - Circulation Supply & Free-Float Supply Ratio (25 pts)**


## This section aims to evaluate… 


## ** \
Answer:** \
 \
**Score: **


<table>
  <tr>
   <td><strong>Score</strong>
   </td>
   <td><strong>Description</strong>
   </td>
  </tr>
  <tr>
   <td>25
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>20
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>15
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>10
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>5
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>0
   </td>
   <td>
   </td>
  </tr>
</table>


**2.5 Adoption - Number of Exchange Listings & Pools (25 pts)**


## Stablecoin adoption can further be measured by adding up all venues where the coin is operational. This can be centralized exchange listings, DEX pairs, lending market pools, and other DeFi use cases.


## ** \
Answer:** \
 \
**Score: **


<table>
  <tr>
   <td><strong>Score</strong>
   </td>
   <td><strong>Description</strong>
   </td>
  </tr>
  <tr>
   <td>25
   </td>
   <td>50+ CEX Listings, 100+ DEX trading pairs, 25+ other pools/vaults
   </td>
  </tr>
  <tr>
   <td>20
   </td>
   <td>25+ CEX Listings, 75+ DEX trading pairs, 15+ other pools/vaults
   </td>
  </tr>
  <tr>
   <td>15
   </td>
   <td>10+ CEX Listings, 50+ DEX trading pairs, 10+ other pools/vaults
   </td>
  </tr>
  <tr>
   <td>10
   </td>
   <td>2+ CEX Listings, 25+ DEX trading pairs, 5+ other pools/vaults
   </td>
  </tr>
  <tr>
   <td>5
   </td>
   <td>No CEX Listing, 10+ DEX trading pairs, 2+ other pools/vaults
   </td>
  </tr>
  <tr>
   <td>0
   </td>
   <td>No CEX Listing, less than 10 DEX pairs, no other relevant pools/vaults
   </td>
  </tr>
</table>


**2.6 Adoption - Number of Stablecoin Holders (25 pts)**


## This measures adoption simply by looking at the total amount of token holders. 


## ** \
Answer:** \
 \
**Score: **


<table>
  <tr>
   <td><strong>Score</strong>
   </td>
   <td><strong>Description</strong>
   </td>
  </tr>
  <tr>
   <td>25
   </td>
   <td>More than 2M holders
   </td>
  </tr>
  <tr>
   <td>20
   </td>
   <td>More than 500k holders
   </td>
  </tr>
  <tr>
   <td>15
   </td>
   <td>More than 100k holders
   </td>
  </tr>
  <tr>
   <td>10
   </td>
   <td>More than 25k holders
   </td>
  </tr>
  <tr>
   <td>5
   </td>
   <td>More than 2.5k holders
   </td>
  </tr>
  <tr>
   <td>0
   </td>
   <td>Less than 2.5k holders
   </td>
  </tr>
</table>


**2.3 Activity - Market Share Growth (25 pts)**


## This section aims to evaluate recent stablecoin activity by measuring its growth rate. Since market share is a highly representative key metric of user adoption, it’s growth rate represents an insightful parameter to quantify recent changes in usage.


## ** \
Answer:** \
 \
**Score: **


<table>
  <tr>
   <td><strong>Score</strong>
   </td>
   <td><strong>Description</strong>
   </td>
  </tr>
  <tr>
   <td>25
   </td>
   <td>30d growth rate +250%
   </td>
  </tr>
  <tr>
   <td>20
   </td>
   <td>30d growth rate +100%
   </td>
  </tr>
  <tr>
   <td>15
   </td>
   <td>30d growth rate +50%
   </td>
  </tr>
  <tr>
   <td>10
   </td>
   <td>30d growth rate +20%
   </td>
  </tr>
  <tr>
   <td>5
   </td>
   <td>30d growth rate +5%
   </td>
  </tr>
  <tr>
   <td>0
   </td>
   <td>No growth rate
   </td>
  </tr>
</table>


**2.4 Activity - Daily Transactions (25 pts)**


## This section aims to evaluate a stablecoins activity by taking into account the number of daily transactions.


## ** \
Answer:** \
 \
**Score: **


<table>
  <tr>
   <td><strong>Score</strong>
   </td>
   <td><strong>Description</strong>
   </td>
  </tr>
  <tr>
   <td>25
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>20
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>15
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>10
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>5
   </td>
   <td>
   </td>
  </tr>
  <tr>
   <td>0
   </td>
   <td>
   </td>
  </tr>
</table>



# **3. Peg Stability - 150 pts**



* Price (off-peg) deviation % - over 7d, 30d, 60d, 90d and 180d -
* Price (off-peg) deviation % on historical “black swan” events -
* Days in operation (>1000 days = max points, 800-1000 days 75% points, 500-800… etc)


# **4. Stabilization mechanism score**



* Issuance and redemption mechanisms
* Protocol/DAO/Company controlled stability mechanisms (internal mechanisms)
* Open market stability mechanisms (market mechanisms)
* Complexity (0 - highly complex mechanism, 25 - simple mechanism)


# **5. Collateral Quality score - 100 pts**



* Collateral structure (diversification level)
* Capital efficiency (average CR in %) -
* Collateral volatility
* Collateral liquidity
* Scalability - how much is the total market capitalization of all eligible collateral? (the higher the more points, e.g. LUSD is limited to ETH, so the market cap of ETH - CR is the maximum market cap of LUSD. USDC is much higher because fiat is technically infinite)


# **6. Technical security score - 100 pts**



* Smart Contract Audits and Bug Bounty Programs (external auditors and influence) - 40 pts
* Smart Contract Architecture quality and complexity (internal factors - team members, contributors, forked code level, ) - 40 pts
* The technical risk from integrated protocols (Composability risk - technical side) - 20 pts
* Can hint at a collaboration with DeFi Safety at a later stage
* Minus points for exploits/hacks
* 


# **7. Regulation score - 50 pts**



* Fragility degree in different regulatory scenarios (categorization of different regulatory directions and potential influence on stablecoin stability and usability) - 0 - regulatory change has a high impact on the stablecoin, 50 - regulatory change hasn't impact on stablecoin. 50 pts

Metrics in green color can be added later (can also add it now, but leave the metric blanks or “soon”)

**Sources**

MakerDAO metrics [https://dune.com/SebVentures/maker---accounting_1](https://dune.com/SebVentures/maker---accounting_1)


# Stablecoin Classification


<table>
  <tr>
   <td colspan="8" ><strong>Non-custodial / Off-chain Collateralized Stablecoins</strong>
   </td>
  </tr>
  <tr>
   <td><strong>Custody</strong>
   </td>
   <td><strong>Collateralization ratio</strong>
   </td>
   <td><strong>Collateral Category</strong>
   </td>
   <td><strong>Collateral-type</strong>
   </td>
   <td><strong>Issuer-type</strong>
   </td>
   <td><strong>Issuer</strong>
   </td>
   <td><strong>Decentralisation</strong>
   </td>
   <td><strong>Example</strong>
   </td>
  </tr>
  <tr>
   <td rowspan="5" >Off-chain (custodial)
   </td>
   <td rowspan="4" >Collateralized (1:1)
   </td>
   <td>Fiat-backed
   </td>
   <td>- US-Dollar
   </td>
   <td>Unregulated limited liability company (<a href="https://en.wikipedia.org/wiki/Tether_(cryptocurrency)">Hong Kong-based</a>)
   </td>
   <td><a href="https://tether.to/en/">Tether Limited</a>
   </td>
   <td>100% centralized
   </td>
   <td>USDT
   </td>
  </tr>
  <tr>
   <td rowspan="3" >Fiat-backed + cash equivalents
   </td>
   <td rowspan="3" >- US-Dollar \
- Short-dated U.S. treasuries
   </td>
   <td>US-based private company (with <a href="https://en.wikipedia.org/wiki/Circle_(company)">BitLicense</a> from state of NY)
   </td>
   <td><a href="https://www.circle.com/en/usdc">Circle</a>
   </td>
   <td>100% centralized
   </td>
   <td>USDC
   </td>
  </tr>
  <tr>
   <td rowspan="2" >Limited-purpose trust charter (U.S. regulated)
   </td>
   <td>Paxos Trust Company (for Binance)
   </td>
   <td>100% centralized
   </td>
   <td>BUSD
   </td>
  </tr>
  <tr>
   <td>Paxos Trust Company
   </td>
   <td>100% centralized
   </td>
   <td>USDP
   </td>
  </tr>
  <tr>
   <td>Under- collateralized
   </td>
   <td>Trust-backed + fiat & securities
   </td>
   <td>- Cash equivalents
<p>
- Forex
<p>
- Government Bonds
<p>
- Securities
   </td>
   <td>Government-backed financial institution
   </td>
   <td>Central Banks
   </td>
   <td>100% centralized
   </td>
   <td>CBDC
   </td>
  </tr>
</table>



<table>
  <tr>
   <td colspan="8" ><strong>Non-Custodial / On-chain Collateralized Stablecoins</strong>
   </td>
  </tr>
  <tr>
   <td><strong>Custody</strong>
   </td>
   <td><strong>Collateralization ratio</strong>
   </td>
   <td><strong>Collateral Category</strong>
   </td>
   <td><strong>Collateral-type</strong>
   </td>
   <td><strong>Issuer-type</strong>
   </td>
   <td><strong>Issuer</strong>
   </td>
   <td><strong>Decentralisation</strong>
   </td>
   <td><strong>Example</strong>
   </td>
  </tr>
  <tr>
   <td rowspan="5" >On-chain (non- custodial)
   </td>
   <td rowspan="3" >Over-
<p>
Collateralized (150-250%)
   </td>
   <td>Crypto + RWA (soon)
   </td>
   <td>- USDC
<p>
- ETH
<p>
- WBTC \
- LINK
<p>
- stETH
<p>
- G-Uni
<p>
- rETH
<p>
- RWA
   </td>
   <td>Ethereum-based Protocol
   </td>
   <td>MakerDAO
   </td>
   <td>40% decentralized
   </td>
   <td>DAI
   </td>
  </tr>
  <tr>
   <td>Crypto-backed
   </td>
   <td>- ETH
   </td>
   <td>Ethereum-based Protocol
   </td>
   <td>Liquity
   </td>
   <td>100% decentralized
   </td>
   <td>LUSD
   </td>
  </tr>
  <tr>
   <td>Yield-bearing tokens
   </td>
   <td>- yvWETH
<p>
- yvcrvIB
<p>
- crv3pool
<p>
- xSushi
<p>
- sSpell
   </td>
   <td>Ethereum-based Protocol
   </td>
   <td>Magic Internet Money
   </td>
   <td>100% decentralized
   </td>
   <td>MIM
   </td>
  </tr>
  <tr>
   <td>Over-
<p>
Collateralized (350-400%)
   </td>
   <td>Governance token
   </td>
   <td>- SNX
   </td>
   <td>Ethereum-based Protocol
   </td>
   <td>Synthetix
   </td>
   <td>100% decentralized
   </td>
   <td>sUSD
   </td>
  </tr>
  <tr>
   <td>Collateralized (1:1)
   </td>
   <td>Crypto-backed
   </td>
   <td>- DAI
   </td>
   <td>Ethereum-based Protocol
   </td>
   <td>Tribe DAO
   </td>
   <td>70% decentralized
   </td>
   <td>FEI
   </td>
  </tr>
</table>



<table>
  <tr>
   <td colspan="8" ><strong>Algorithmic Stablecoins</strong>
   </td>
  </tr>
  <tr>
   <td><strong>Custody</strong>
   </td>
   <td><strong>Collateralization ratio</strong>
   </td>
   <td><strong>Collateral Category</strong>
   </td>
   <td><strong>Collateral-type</strong>
   </td>
   <td><strong>Issuer-type</strong>
   </td>
   <td><strong>Issuer</strong>
   </td>
   <td><strong>Decentralisation</strong>
   </td>
   <td><strong>Example</strong>
   </td>
  </tr>
  <tr>
   <td rowspan="2" >On-chain
   </td>
   <td>No collateral (0%)
   </td>
   <td>n/a
   </td>
   <td>n/a
   </td>
   <td>Ethereum-based self-reflexive smart contract (elastic supply model)
   </td>
   <td>Ampleforth
   </td>
   <td>100% decentralized
   </td>
   <td>AMPL
   </td>
  </tr>
  <tr>
   <td>No collateral (0%)
   </td>
   <td>n/a
   </td>
   <td>n/a
   </td>
   <td>Ethereum-based self-reflexive smart contract (elastic supply model)
   </td>
   <td>Empty Set Finance
   </td>
   <td>100% decentralized
   </td>
   <td>ESD
   </td>
  </tr>
</table>



<table>
  <tr>
   <td colspan="8" ><strong>Hybrid Stablecoins</strong>
   </td>
  </tr>
  <tr>
   <td><strong>Custody</strong>
   </td>
   <td><strong>Collateralization ratio</strong>
   </td>
   <td><strong>Collateral Category</strong>
   </td>
   <td><strong>Collateral-type</strong>
   </td>
   <td><strong>Issuer-type</strong>
   </td>
   <td><strong>Issuer</strong>
   </td>
   <td><strong>Decentralisation</strong>
   </td>
   <td><strong>Example</strong>
   </td>
  </tr>
  <tr>
   <td>On-chain (non- custodial)
   </td>
   <td>Fractional- argorithmic
<p>
(93.25% 
<p>
collateralized & 6.76% algorithmic)
   </td>
   <td>Crypto-backed + secondary token (FXS)
   </td>
   <td>- USDC
<p>
- Lending AMOs
<p>
- Investor AMOs
<p>
- Liquidity AMOs
<p>
- Curve AMOs
<p>
- FXS
   </td>
   <td>Ethereum-based Protocol
   </td>
   <td>Frax
   </td>
   <td>13% decentralized
   </td>
   <td>FRAX
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
</table>

