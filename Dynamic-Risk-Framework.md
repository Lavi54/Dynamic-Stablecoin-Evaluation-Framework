


**Date**: 		December 13th, 2022

**Authors**: 	[Lavi](https://twitter.com/Lavi_54) & [Dabar90](https://twitter.com/dabar_90)


# A Dynamic Stablecoin Evaluation Framework


## Abstract

This concept presents a framework for evaluating stablecoin projects. Stablecoins are cryptocurrencies that are pegged to a stable asset, such as the US dollar, to reduce volatility and provide a stable store of value. The framework is designed to create a holistic overview of stablecoin projects and to enable comparison between them by setting a standard. It also aims to facilitate risk assessments and enable real-time health metrics. The first three categories of the framework are based on the stablecoin trilemma in combination with standard fundamental analysis concepts, to identify the quality and risks of stablecoin protocols.


## Introduction

Stablecoins are cryptocurrencies that are pegged to a stable asset, such as the US dollar. Typically their main purpose is to reduce volatility and provide a stable store of value. However, stablecoins have faced several challenges and criticisms. One of the main issues is that the peg to the underlying asset is not always reliable. Another problem is that some of the most prominent stablecoins are issued by private companies. Many projects issuing decentralized stablecoins on the other hand still lack wider adoption. Besides these fundamental issues, many other risks come with financial primitives in web3.

Despite these challenges, the use of stablecoins is growing. In fact, stablecoins are one of the most important innovations in DeFi, with one of the highest addressable markets of all use cases. Thus, the number of projects issuing stablecoins is also growing rapidly. 

However, very little has been done in terms of identifying, articulating, or measuring the risks related to those projects. It’s very difficult for users to accentuate the quality of today’s stablecoin landscape. With this whitepaper, we aim to create a foundation for defining an evaluation framework for stablecoins. Primarily to facilitate identifying and measuring all relevant components that can be used to measure the quality and potentially certain risks related to these protocols.

In essence, this documentation will provide a detailed explanation of how stablecoins can be evaluated. The objectives of this whitepaper are as follows:



1. Create a holistic overview of all relevant aspects of stablecoin projects.
2. Enable comparison between stablecoins by setting a standard.
3. Facilitate risk assessments and enable real-time health metrics.


## An Approach to Creating a Risk Framework

To achieve these objectives, we first need to create a holistic overview of all relevant aspects of stablecoin projects. In other words, what components are required for a stablecoin project to become viable, and in an ideal scenario, become a sustainably viable alternative to fiat money. We largely base the core pillars around the stablecoin trilemma. In addition, we apply standard fundamental analysis concepts that help identify the quality and risks of stablecoin protocols.

In the second step, we need to make all relevant components measurable. For this, we fully rely on publicly available metrics. Basing the evaluation framework on fundamental key metrics introduces an objective foundation to calculate the scores. In return, we forgo certain equally important dimensions (e.g. the team or community). These are more complicated to measure and thus more difficult to compare objectively. Hence, we postpone coverage of these aspects to a later version.

Still, it is tricky to fully eliminate subjective assumptions. Despite only using public key metrics, subjectivity comes into play when weighing the scores. Essentially the final score of a project is decided by how well it scored per category, in combination with how much each category contributes to the overall score. For this system to be representative, and as close to the truth as possible, we have to set a clear perspective. While trying to strike the right balance between all components, we essentially lean more toward the perspective of stablecoin users.

Hence, the main focus is on existing or potential risks for stablecoin holders. The framework is not targeted toward governance token holders, or investors of the entity issuing the stablecoin. Therefore, we first and foremost pay attention to components that, from our point of view, pose a risk to end users of the stablecoin. For example, we assume that decentralization is important, and that centralization can pose a risk. Hence, it is weighted slightly higher than scalability. But we will explain the weighting in more detail below.

Before diving into the framework, we first want to be able to clearly differentiate between different categories of stablecoins. The classification system presented in the next section builds the basis for this.


## Stablecoin Classification

To facilitate the differentiation between stablecoin projects, we use a classification system. This will provide high-level separation and introduce subcategories for further separation. At the start, the framework itself will not apply the categorization and it will not differentiate between different stablecoin categories. As mentioned in the first section, our objective is to make stablecoins comparable. Thus, it is essential that the same evaluation framework is used as a basis. The drawback of this approach is that certain important factors that might differentiate a certain category are not measured or might not be weighted in favour of said categories. Later iterations of this framework can then be customized to better suit a specific category.

In the meantime, we are going to recognize the following four stablecoins categories.



1. **Custodial Stablecoins**

    These are stablecoins where the assets are stored off-chain. Typically one centralized entity has custody of the collateral assets (examples: USDT, USDC).

2. **Non-custodial Stablecoins**

    This category includes all stablecoin protocols that have their collateral on-chain. This is typically referred to as non-custodial, meaning that the collateral is held by smart contracts (examples: DAI, LUSD, sUSD).

3. **Algorithmic Stablecoins**

    This category refers to fully algorithmic “stablecoins” that don’t require collateral-backing. Some see this as the holy grail of stablecoins. However, the quotation marks hint at the fact that none of these projects have achieved price stability so far (examples: AMPL, ESD)

4. **Hybrid Stablecoins**

    This last category encompasses projects that apply a mix of algorithmic and collateral-backed methods to create a stable asset (examples: FRAX).


The second, third, and fourth category tiers take into consideration the collateralization ratio, the collateral type, and finally their issuer type. The full category overview including some examples is in the appendix at the end of this document.

For readers already familiar with the stablecoin trilemma, we recommend skipping the next section and moving directly to the Evaluation Framework Overview.


## The Stablecoin Trilemma

Before diving into the evaluation framework, it’s essential that the reader understands the stablecoin trilemma, as we’ll be basing the first three sections on this problem statement.

The stablecoin trilemma describes the three problems that a stablecoin needs to solve, for it to become a viable alternative to fiat money. The three problems are price stability, decentralization, and scalability (capital efficiency).



<p id="gdcalert1" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image1.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert2">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image1.png "image_tooltip")


(Source: [Twitter](https://twitter.com/chainlinkgod/status/1528954630813667328))

As of today, no stablecoin embodies all three simultaneously at scale. Typically, stablecoin projects neglect one component in favour of the other two. For instance, USDC and USDT are highly scalable and the most used stablecoin. But they are 100% custodial and centralized. The collateral that is backing these stables is stored off-chain and custody is with centralized entities. This poses the risk of a single point of failure. Moreover, this setup is not censorship-resistant. Circle has already blacklisted certain addresses from using their stablecoin USDC.

DAI, for instance, was initially targeted to be a fully decentralized stablecoin. However, this objective was relinquished over the years, as the community had difficulties scaling the project when only accepting ETH as collateral. To solve this, they started to accept centralized USDC as backing. As a result, some say that DAI is more like wUSDC, with over 60% of DAI being backed by USDC. While Maker is a decentralized protocol, it has to rely on centralized collateral. Moreover, it uses over-collateralized CDP’s to ensure security and price stability. This makes DAI capital inefficient. Meaning that more value has to be locked than can be issued in DAI.

There is also the drastic example of Terra and UST. This project scaled very fast and it was somewhat decentralized. But to achieve this, the project applied a reflexive backing system, with LUNA as the only collateral. LUNA was minted or burned, depending on the demand for UST. Essentially, this led to a death-spiral event, when UST depegged and more LUNA had to be minted than the market was able to absorb. In other words, UST neglected price stability for the sake of scalability.

In conclusion, we found that this trilemma provides a suitable foundation to create a review framework. It’s a fair compromise to base the evaluation on, as all stablecoin projects have to face these same three issues in their initial design. We believe that an evaluation system should award the projects that solve these problems well.

Of course, there are more issues and risk vectors in the actual implementation and we have augmented the scoring system with additional scoring categories. The next section will explain all categories in more detail.


## Evaluation Framework Overview

In its first version, the review framework will assess stablecoins based on five main categories. As mentioned above, the first three categories are based on the stablecoin trilemma. They aim to evaluate how well a project solves each of the three problems described above. The fourth category is used to provide an in-depth understanding of the collateral that is backing the stablecoin. The last category aims to provide insights into the technical quality of the protocol.


### 1. Decentralization

The first section of the framework tries to evaluate a protocol's path to decentralization. While decentralization can be understood and defined in different ways, it is mainly the opposite (i.e. centralization)that makes this section quantifiable. For instance, while there is no agreement yet on what “full decentralization” looks like, there is agreement that only 10 nodes securing a network is considered a centralized blockchain.

In the same manner, we try to measure how “decentralized” a stablecoin project is. The first question will focus on the issuer of the token. On one side there are centralized stablecoin issuers and on the other DAO-governed stablecoin cannot be controlled by one single entity (or a group of few actors). 

The second pillar is the stablecoin users. For this question, the wealth distribution can provide insights into who’s using the stablecoin. Finally, the collateral decentralization ratio (CDR) measures the centralization risk of the collateral. Collateral with excessive off-chain risk (e.g. fiat-backed stables or custodial assets such as gold/oil etc.) is considered to be 0% decentralized. ETH as well as certain reward tokens such as AAVE or CRV are counted as 100% decentralized.


### 2. Scalability / Capital Efficiency

Measuring effective scalability as in “its potential for exponential and fast growth”, requires the placement of proxy indicators. Hence, we use a project's current adoption rate as the foundation to measure its potential for sustainable and exponential growth.

The adoption can easily be measured by evaluating a project’s user base, market share, and average daily transactions. Further, the acceptance of a stablecoin as means of payment is indicated by how widely it is adapted as a trading pair or other DeFi-related use cases. Thus, CEX listings, DEX pools, as well as lending pools, and yield-generating vaults are considered and awarded. 


### 3. Price Stability

The last of the three trilemma components is mainly measured by looking at a project's historic performance. It can be argued that crypto markets had their fair share of black swan events, market distress, and high volatility. Thus, considering historic performance is deemed as a good indicator of the stablecoins price stability.

In addition, a confidence rating is given concerning the project's stability mechanisms. In general, multiple mechanisms that complement each other and that are well incentivized are considered safer than just relying on arbitrage for example. Over-collateralization, for instance, is considered to be safer than 1:1 or under-collateralization.


### 4. Collateral Quality

The underlying collateral is another essential part. It touches on all three aspects of the stablecoin trilemma. For instance, when using centrally issued currencies as backing, it influences the decentralization ratio. Relying on collateral with low availability can impact the scalability of the project. And when using highly volatile or low-quality tokens to back the stablecoin, it can affect the price stability.

Essentially, this section measures the quality of the collateral by dividing it into quality tiers. However, collateral cannot be looked at in isolation, which is why the structure - or collateral diversification - is equally important. As mentioned above, capital efficiency also plays a key role, whereby over-collateralization is deemed inefficient. Highly volatile collateral is also deemed less “fit for purpose” than more stable collateral.

Finally, the section also evaluates a project's transparency, by defining how easy it is to “audit” the collateral, i.e. to confirm that the backing is actually there.


### 5. Technical Security

As with all projects that rely on smart contracts, code quality, and technical sophistication is very important risk vectors. Most hacks or exploits happen due to technical issues and unheeding security.

While technical security is a field of investigation in itself, some proxy metrics can be abstracted to get a fair impression of a project's technical safety. The first is smart contract audits, which are measured by looking at the number of audits, the time passed, and finally combined with a subjective statement on the audit firm's reputation. Another important measure to prevent smart contract vulnerabilities is bug bounty programs. This can again easily be quantified by looking at the dollar amount of the bounty in relation to the TVL that the protocol holds. Finally, testing can help to circumvent economic as well as technical issues. Hence, thorough testing and verification processes are taken into account.

Lastly, this section has a unique section that can result in minus points. That is, the hack or exploit penalty will subtract a certain amount from the protocol’s total score, depending on the amount and severity of the exploits.


## Closing Statement

As mentioned above, this risk framework aims to be as objective as possible. It also aims to be dynamic. Thus, we start with a rather lean version. We forgo the inclusion of other relevant dimensions, to first prove the viability of this basic version. Other fundamental aspects such as team, governance, partnerships, or regulatory risks shall be added in later versions. The current version is also limited by data availability. That is, in order for this framework to become fully dynamic and independent of manual updates, it requires the right data streams to feed its algorithm. This first iteration still relies on a few manual and rather subjective scoring components, however, already now the majority of the scores can be retrieved directly on-chain or from certain data providers.

Furthermore, we also aim to introduce the evaluation of yield-bearing synthetic stablecoin representations, such as aDAI or cUSDC for instance. This will require the rather extensive evaluation of the lending protocol (e.g. Aave and Compound), which is also deferred to a later stage of this project. However, in combination, this will then allow a full risk-return rating system. In other words, yield can be put in contrast to its associated risk. This will be powerful.




# **Stablecoin Evaluation Framework**


# **Overview **

The overview section should provide a high-level introduction to the project. This helps to prepare the reader for what type of project the report is about. A good approach is to summarise the key activities of the protocol and summarise the findings of each section at the end.


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
   <td>X / 100
   </td>
  </tr>
  <tr>
   <td>1.2
   </td>
   <td>User Distribution
   </td>
   <td>X / 50
   </td>
  </tr>
  <tr>
   <td>1.3
   </td>
   <td>Collateral Decentralization Ratio (CDR)
   </td>
   <td>X / 50
   </td>
  </tr>
  <tr>
   <td colspan="2" ><strong>Total Decentralization Score</strong>
   </td>
   <td><strong>X / 200</strong>
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
   <td>Stablecoin Market Share
   </td>
   <td>X / 30
   </td>
  </tr>
  <tr>
   <td>2.2
   </td>
   <td>Circulating and Free Float Supply Ratio
   </td>
   <td>X / 30
   </td>
  </tr>
  <tr>
   <td>2.3
   </td>
   <td>Number of Exchange Listings & Pools
   </td>
   <td>X / 30
   </td>
  </tr>
  <tr>
   <td>2.4
   </td>
   <td>Number of Stablecoin Holders
   </td>
   <td>X / 30
   </td>
  </tr>
  <tr>
   <td>2.5
   </td>
   <td>Average Daily Transactions
   </td>
   <td>X / 30
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
   <td>Price (off-peg) deviation
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
   <td>Days in Operation
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
   <td>Collateral Quality
   </td>
   <td>X / 30
   </td>
  </tr>
  <tr>
   <td>4.2
   </td>
   <td>Capital Structure/Diversification
   </td>
   <td>X / 30
   </td>
  </tr>
  <tr>
   <td>4.3
   </td>
   <td>Capital Efficiency
   </td>
   <td>X / 30
   </td>
  </tr>
  <tr>
   <td>4.4
   </td>
   <td>Collateral Volatility
   </td>
   <td>X / 30
   </td>
  </tr>
  <tr>
   <td>4.5
   </td>
   <td>
<h2>Auditability of the Collateral</h2>


   </td>
   <td>X / 30
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
   <td>Smart Contract Audits 
   </td>
   <td>X / 50
   </td>
  </tr>
  <tr>
   <td>4.2
   </td>
   <td>Bug Bounty Programs
   </td>
   <td>X / 50
   </td>
  </tr>
  <tr>
   <td>4.3
   </td>
   <td>Testing
   </td>
   <td>X / 50
   </td>
  </tr>
  <tr>
   <td>4.4
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


**Rating Table**


<table>
  <tr>
   <td><strong>Rating</strong>
   </td>
   <td><strong>Description</strong>
   </td>
   <td><strong>Score</strong>
   </td>
  </tr>
  <tr>
   <td>AA
   </td>
   <td>Prime-grade protocol
   </td>
   <td>Total Score >85%
   </td>
  </tr>
  <tr>
   <td>A
   </td>
   <td>High-grade protocol
   </td>
   <td>Total Score >75%
   </td>
  </tr>
  <tr>
   <td>BB
   </td>
   <td>Upper-medium-grade protocol
   </td>
   <td>Total Score >60%
   </td>
  </tr>
  <tr>
   <td>B
   </td>
   <td>Medium-grade protocol
   </td>
   <td>Total Score >50%
   </td>
  </tr>
  <tr>
   <td>CC
   </td>
   <td>Lower-medium-grade protocol
   </td>
   <td>Total Score >40%
   </td>
  </tr>
  <tr>
   <td>C
   </td>
   <td>Low-grade protocol
   </td>
   <td>Total Score >30%
   </td>
  </tr>
  <tr>
   <td>D
   </td>
   <td>Garbage
   </td>
   <td>TotalScore &lt;30%
   </td>
  </tr>
</table>






1. **Decentralization - 200 pts**

This first section aims to capture a stablecoins progress toward decentralization. Typically a project starts rather centralized, with the founding team having strong influence. However, as the projects mature, dependency on the team and other centralized parties should diminish. The immutability of core smart contracts can also reduce reliance and thus, reduce risks of harmful changes.

**1.1 Decentralized Issuer/Governance (100 pts)**


## Distributed governance allows token holders and community members to participate in the governance of open finance protocols. This section tries to identify whether a stablecoin’s governance system is sufficiently decentralized. To answer this, the question to be asked is: “can one entity, or a small group, exert significant influence over the stablecoin or the protocol? This can be either via exclusive access rights to core functionalities (e.g. smart contracts) or a high concentration of voting power.


## This first section is only relevant to non-custodial protocols. Fiat-backed stables with off-chain collateral will get 0 points.


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
   <td>100
   </td>
   <td>Voting power is substantially decentralized, there is a large and active community, and no central party or small group has majority voting power.
   </td>
  </tr>
  <tr>
   <td>75
   </td>
   <td>Voting power is fairly decentralized, there is an active community, and no central party has majority voting power.
   </td>
  </tr>
  <tr>
   <td>50
   </td>
   <td>Voting power is somewhat decentralized or somewhat concentrated around a few addresses. Those are well-known and trusted community members.
   </td>
  </tr>
  <tr>
   <td>25
   </td>
   <td>Governance is rather centralized. The community can take influence, but voting power is in the hands of a few.
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


**1.2 User Distribution (50 pts)**


## The user distribution can help to better understand the usage of a stablecoin. If there is a high supply concentration, this typically hints that the coin is mostly used by a few large holders. And less established for retail use cases. To measure the distribution, the total number of addresses, that together hold 80% or more of the total supply, is measured.


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
   <td>80% of total supply is held by 1500 or more addresses
   </td>
  </tr>
  <tr>
   <td>40
   </td>
   <td>80% of total supply is held by 750 or more addresses
   </td>
  </tr>
  <tr>
   <td>30
   </td>
   <td>80% of total supply is held by 250 or more addresses
   </td>
  </tr>
  <tr>
   <td>20
   </td>
   <td>80% of total supply is held by 100 or more addresses
   </td>
  </tr>
  <tr>
   <td>10
   </td>
   <td>80% of total supply is held by less than 50 addresses
   </td>
  </tr>
  <tr>
   <td>0
   </td>
   <td>80% of total supply is held by less than 10 addresses
   </td>
  </tr>
</table>


**1.3 Collateral Decentralization Ratio (50 pts)**


## The entity issuing a stablecoin might be decentralized, censorship-resistant, and fully immutable. However, there is little value in that when the collateral is subject to significant centralized control.


## The collateral decentralization ratio (CDR) measures the centralization risk of collateral tokens. Collateral with excessive off-chain risk (e.g. fiat-backed stables or custodial assets such as gold/oil etc.) is considered to be 0% decentralized. ETH or MATIC, as well as certain reward tokens such as AAVE or CRV, are counted as 100% decentralized.


## The question is whether the collateral is subject to centralized authority and whether the authority has the potential to blacklist or otherwise limit usage, and thus change its viability as collateral.


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


## This section aims to evaluate stablecoins scalability and efficiency. Scalability is not easily quantifiable, hence the current adoption and overall acceptance of the stable as the method of payment is used as a proxy.

**2.1 Stablecoin Market Share (30 pts)**


## The market share is used to quantify a stablecoins rank when compared with its peers and competitors.


## ** \
Answer: ** \



## **Score: **


<table>
  <tr>
   <td><strong>Score</strong>
   </td>
   <td><strong>Description</strong>
   </td>
  </tr>
  <tr>
   <td>30
   </td>
   <td>Market leader = Highest market share
   </td>
  </tr>
  <tr>
   <td>25
   </td>
   <td>Strong competitor = 2nd or 3rd highest market share
   </td>
  </tr>
  <tr>
   <td>20
   </td>
   <td>Established market participant = ranking 4-8 in terms of market share
   </td>
  </tr>
  <tr>
   <td>15
   </td>
   <td>New entrant/weak competitor = ranking 9-20 market share
   </td>
  </tr>
  <tr>
   <td>10
   </td>
   <td>Lower-end competitor = ranking 21 to 40 market share
   </td>
  </tr>
  <tr>
   <td>5
   </td>
   <td>Functional but not established = ranking 40 and lower
   </td>
  </tr>
  <tr>
   <td>0
   </td>
   <td>Fake, scam, or otherwise not usable
   </td>
  </tr>
</table>


**2.2 Circulation Supply & Free-Float Supply Ratio (30 pts)**


## This section aims to evaluate the free-float supply of each stablecoin. FFSR is calculated as circulating supply minus the tokens still locked in the issuer contract. This provides a more accurate picture of tokens in actual usage than just looking at the circulating supply.


## ** \
Answer:**  \
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
   <td>30
   </td>
   <td>100B+ of FFSR
   </td>
  </tr>
  <tr>
   <td>25
   </td>
   <td>10B+ of FFSR
   </td>
  </tr>
  <tr>
   <td>20
   </td>
   <td>1B+ of FFSR
   </td>
  </tr>
  <tr>
   <td>15
   </td>
   <td>100M+ of FFSR
   </td>
  </tr>
  <tr>
   <td>10
   </td>
   <td>10M+ of FFSR
   </td>
  </tr>
  <tr>
   <td>5
   </td>
   <td>1M+ of FFSR
   </td>
  </tr>
  <tr>
   <td>0
   </td>
   <td>Less than 1M tokens in circulation
   </td>
  </tr>
</table>


**2.3 Number of Exchange Listings & Pools (30 pts)**


## Stablecoin adoption can further be measured by adding up all venues where the coin is operational. This can be centralized exchanges, DEX pairs, lending market pools, and other DeFi use cases (e.g. Yearn vaults, institutional/not-collateralized lending protocols).


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
   <td>30
   </td>
   <td>50+ CEX Listings, 100+ DEX trading pairs, 25+ other pools/vaults
   </td>
  </tr>
  <tr>
   <td>25
   </td>
   <td>25+ CEX Listings, 75+ DEX trading pairs, 15+ other pools/vaults
   </td>
  </tr>
  <tr>
   <td>20
   </td>
   <td>10+ CEX Listings, 50+ DEX trading pairs, 10+ other pools/vaults
   </td>
  </tr>
  <tr>
   <td>15
   </td>
   <td>2+ CEX Listings, 25+ DEX trading pairs, 5+ other pools/vaults
   </td>
  </tr>
  <tr>
   <td>10
   </td>
   <td>No CEX Listing, 10+ DEX trading pairs, 2+ other pools/vaults
   </td>
  </tr>
  <tr>
   <td>5
   </td>
   <td>No CEX Listing, less than 10 DEX pairs, no other relevant pools/vaults
   </td>
  </tr>
  <tr>
   <td>0
   </td>
   <td>No CEX Listing, less than 5 DEX pairs, no other relevant pools/vaults
   </td>
  </tr>
</table>


**2.4 Number of Stablecoin Holders (30 pts)**


## This question evaluates adoption simply by looking at the total number of token holders. This can be counted over one or multiple chains.


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
   <td>30
   </td>
   <td>More than 5M holders
   </td>
  </tr>
  <tr>
   <td>25
   </td>
   <td>More than 2.5M holders
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


**2.5 Daily Transactions (25 pts)**


## This section aims to evaluate a stablecoins activity by taking into account the number of daily transactions. To account for spikes and drops, the average of the last 30, 60, and 90 days is used.


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
   <td>30
   </td>
   <td>Average 90d trx count 200k+
   </td>
  </tr>
  <tr>
   <td>25
   </td>
   <td>Average 90d trx count 100k+
   </td>
  </tr>
  <tr>
   <td>20
   </td>
   <td>Average 90d trx count 50k+
   </td>
  </tr>
  <tr>
   <td>15
   </td>
   <td>Average 90d trx count 25k+
   </td>
  </tr>
  <tr>
   <td>10
   </td>
   <td>Average 90d trx count 5k+
   </td>
  </tr>
  <tr>
   <td>5
   </td>
   <td>Average 90d trx count 1k+
   </td>
  </tr>
  <tr>
   <td>0
   </td>
   <td>Less than 1k daily trx on 90-day average
   </td>
  </tr>
</table>





# **3. Peg & Stability Mechanism - 150 pts**

**3.1 Average Price Deviation (30 pts)**


## Price deviation refers to periods where the stablecoin is off-peg. It’s measured using the highest  standard deviation over the past 90 days.


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
   <td>30
   </td>
   <td>Peg deviation in a range of 0.5% for 90 days period
   </td>
  </tr>
  <tr>
   <td>25
   </td>
   <td>Peg deviation in a range of 1% for 90 days period
   </td>
  </tr>
  <tr>
   <td>20
   </td>
   <td>Peg deviation in a range of 2.5% for 90 days period
   </td>
  </tr>
  <tr>
   <td>15
   </td>
   <td>Peg deviation in a range of 5% for 90 days period
   </td>
  </tr>
  <tr>
   <td>10
   </td>
   <td>Peg deviation in a range of 10% for 90 days period
   </td>
  </tr>
  <tr>
   <td>5
   </td>
   <td>Peg deviation went out of range of 10% multiple times in 90 days period
   </td>
  </tr>
  <tr>
   <td>0
   </td>
   <td>Peg deviation is out of range of 10% constantly in 90 days period
   </td>
  </tr>
</table>


**3.2 Price Deviation during Black Swan Events (25 pts)**


## Keeping the peg during “normal” market conditions is essential, but even more meaningful is stability during market distress (e.g. Black Thursday - 12th of March 2020).


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
   <td>30
   </td>
   <td>Price stayed pegged inside 2.5% deviation during all market “Black Swan” events
   </td>
  </tr>
  <tr>
   <td>25
   </td>
   <td>Price stayed pegged inside 5% deviation during all market “Black Swan” events
   </td>
  </tr>
  <tr>
   <td>20
   </td>
   <td>Price stayed pegged inside 10% deviation during all market “Black Swan“ events
   </td>
  </tr>
  <tr>
   <td>15
   </td>
   <td>Price stayed pegged inside 20% deviation during all market “Black Swan“ events
   </td>
  </tr>
  <tr>
   <td>10
   </td>
   <td>Price went out off peg of 20% range in one “Black Swan” event
   </td>
  </tr>
  <tr>
   <td>5
   </td>
   <td>Price went out off peg of 20% range in 2 or 3“Black Swan” events
   </td>
  </tr>
  <tr>
   <td>0
   </td>
   <td>Price went out more than 20% of peg in every market stress
   </td>
  </tr>
</table>


**3.3 Days in Operation (25 pts)**


## The “age” of a stablecoin can increase confidence in its viability and security. The older a stablecoin, the less likely that it contains severe bugs or economic weaknesses. Hence, the question is how long ago was it deployed and operational without severe failures.


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
   <td>30
   </td>
   <td>2000+ days
   </td>
  </tr>
  <tr>
   <td>25
   </td>
   <td>1500+ days
   </td>
  </tr>
  <tr>
   <td>20
   </td>
   <td>1080+ days
   </td>
  </tr>
  <tr>
   <td>15
   </td>
   <td>720+ days
   </td>
  </tr>
  <tr>
   <td>10
   </td>
   <td>360+ days
   </td>
  </tr>
  <tr>
   <td>5
   </td>
   <td>180+ days
   </td>
  </tr>
  <tr>
   <td>0
   </td>
   <td>Brand new, or multiple severe incidences refuting its viability
   </td>
  </tr>
</table>


**3.4 Stability Mechanisms (30 pts)**

Stability mechanisms are used to keep a tokens peg. Some are built into the protocol, some rely on internal or external actors. For these crypto-economic systems to function, agents that help stabilize the protocol usually require incentivization. This question attempts to investigate to what extent the stability design promotes peg stability and whether the incentive design functions as intended.

** \
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
   <td>30
   </td>
   <td>The protocol has multiple internal and external stability mechanisms in place (at least 3-4). They are battle-tested, fit for purpose, and safe. All agents are incentivized, independent of market conditions. If a governance token exists, it plays a vital role in stabilizing/ securing the monetary system.
   </td>
  </tr>
  <tr>
   <td>25
   </td>
   <td>The protocol has multiple stability mechanisms in place (at least 2-3). They are battle-tested, fit for purpose, and safe. All agents are incentivized, in most market conditions. If a governance token exists, it plays an important role in stabilizing/ securing the monetary system.
   </td>
  </tr>
  <tr>
   <td>15
   </td>
   <td>The protocol has some stability mechanisms in place (at least 2). They seem to work well. Most agents are incentivized, but only in stable market conditions. If a governance token exists, it plays a role in stabilizing/securing the monetary system.
   </td>
  </tr>
  <tr>
   <td>10
   </td>
   <td>The protocol has one stability mechanism in place. It has worked most of the time. Few or no agents are incentivized. If a governance token exists, it plays a role in stabilizing/securing the monetary system.
   </td>
  </tr>
  <tr>
   <td>5
   </td>
   <td>The protocol has one stability mechanism in place, but it has some flaws. Few or no agents are incentivized. The governance token isn’t relevant.
   </td>
  </tr>
  <tr>
   <td> 0
   </td>
   <td>The protocol has an unreliable stability mechanism, depegs are likely.
   </td>
  </tr>
</table>


**3.5 Issuance & Redemption Mechanism (30 pts)**


## In essence, this question attempts to answer how safe the protocols mechanisms are that issue the stablecoin. For instance, CDPs are considered safer, as they require over-collateralization and in liquidations protect the system from acquiring bad debt in case of default. Hence, over-collateralization, using top-tier assets in combination with well-oiled liquidation mechanisms is considered to increase stability. Whereby more experimental, under-collateralized, or permissioned systems are considered less stable.


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
   <td>30
   </td>
   <td>Stablecoin can permissionlessly be minted against over-collateralization. Battle-tested liquidation mechanisms prevent bad debt. Issuance and redemption are easily accessible, affordable, and user-friendly.
   </td>
  </tr>
  <tr>
   <td>25
   </td>
   <td>Stablecoin can permissionlessly be minted against collateralization. Liquidation mechanisms prevent bad debt. Issuance and redemption are accessible and user-friendly.
   </td>
  </tr>
  <tr>
   <td>15
   </td>
   <td>Stablecoin can be minted against collateralization but requires permission. Liquidation mechanisms prevent bad debt. Issuance and redemption are only accessible to accredited users.
   </td>
  </tr>
  <tr>
   <td>5
   </td>
   <td>Stablecoin is issued by a centralized entity. There is no accessibility for the public and little transparency on how issuance/redemption works.
   </td>
  </tr>
  <tr>
   <td>0
   </td>
   <td>Issuance and redemption are very complicated, liquidation mechanism is not proven.
   </td>
  </tr>
</table>



# **4. Collateral Quality - 150 pts**

**4.1 Collateral Quality (30 pts)**

To facilitate measuring the quality of the collateral, i.e. to avoid full fundamental and risk review of for instance Ethereum or WBTC, the collateral’s market ranking, CEX listings, general sentiment, and adoption will be taken into account. Essentially, we aim to separate between top-tier assets (e.g. ETH, BTC, USDC), high-tier assets (e.g. Uni LPs, CRV LPs), medium-tier assets (e.g. AAVE, CRV, MATIC), and lower-tier assets. To define the tier, external sources such as PrimeRating, Curve, or MakerDAO asset risk assessments are considered as well.


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
   <td>30
   </td>
   <td>Collateral is only top tier (ETH, BTC, USDC)
   </td>
  </tr>
  <tr>
   <td>20
   </td>
   <td>Collateral is mostly top tier and higher tier (e.g. ETH, Uni LPs, Curve LPs)
   </td>
  </tr>
  <tr>
   <td>10
   </td>
   <td>Collateral is high tier and medium tier asset (e.g. Curve LPs, CRV, yDAI)
   </td>
  </tr>
  <tr>
   <td>0
   </td>
   <td>Collateral is mostly low tier assets (e.g. APE, FARM)
   </td>
  </tr>
</table>


**4.2 Collateral Structure/Diversification (30 pts)**

To measure the quality of the collateral backing the stablecoin, it is important to also take into consideration the diversification of the basket backing it. Diversification can decrease the risks for certain collateral and decrease reliance on one or a few collateral types.

If the trust in the monetary system is mainly based on the collateral, a key consideration is an extent to which the collateral is correlated among itself and to crypto markets in general. Since a downturn in collateral could alter the degree of collateralization and cause a bank-run scenario. This is only relevant for volatile collateral. To calculate the correlation between assets, the correlation ratio (r) can be used, whereby r = 1 means fully correlated and r = 0 means no correlation.


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
   <td>30
   </td>
   <td>Collateral is well diversified and not strongly correlated (r &lt; 0.25)
   </td>
  </tr>
  <tr>
   <td>20
   </td>
   <td>Collateral is diversified and only somewhat correlated (r = 0.25 - 0.75)
   </td>
  </tr>
  <tr>
   <td>10
   </td>
   <td>There are only a few collaterals enabled and it’s correlated (r > 0.75)
   </td>
  </tr>
  <tr>
   <td>0
   </td>
   <td>There’s none or very little diversification and collateral is fully correlated (r = 1)
   </td>
  </tr>
</table>


**4.3 Capital Efficiency (30 pts)**


## Certain stablecoin mechanisms are limited by their design configuration to scale. For instance, MakerDAO’s DAI requires over-collateralization to issue fresh DAI. The effect of this is that these stablecoins require more value to be locked than it releases, which is considered capital inefficient.


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
   <td>30
   </td>
   <td>The project is highly capital efficient. No over-collateralization is required and collateral is used productively.
   </td>
  </tr>
  <tr>
   <td>20
   </td>
   <td>The project is somewhat capital efficient (e.g. 1:1 collateralization ratio). Collateral is productive.
   </td>
  </tr>
  <tr>
   <td>10
   </td>
   <td>The project is rather capital inefficient (CR > 120%). But collateral is used productively.
   </td>
  </tr>
  <tr>
   <td>5
   </td>
   <td>The project is capital inefficient (CR > 150%). Collateral is not productive.
   </td>
  </tr>
  <tr>
   <td>0
   </td>
   <td>The project is very inefficient (CR > 250%).
   </td>
  </tr>
</table>


**4.4 Collateral Volatility (30 pts)**


## Measuring the volatility of the collateral indicates how well it is suited to back a stable asset. The higher its volatility the more difficult it becomes to ensure a certain collateralization ratio.


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
   <td>30
   </td>
   <td>Collateral is stable.
   </td>
  </tr>
  <tr>
   <td>20
   </td>
   <td>Collateral is mostly stable with some volatile assets
   </td>
  </tr>
  <tr>
   <td>10
   </td>
   <td>Collateral is rather volatile, with an average 30-day volatility of 5%+
   </td>
  </tr>
  <tr>
   <td>5
   </td>
   <td>Collateral is very volatile, with an average 30-day volatility of 10%+
   </td>
  </tr>
  <tr>
   <td>0
   </td>
   <td>Collateral is extremely volatile, with an average 30-day volatility of 20%+
   </td>
  </tr>
</table>



## **4.5 Auditability of the Collateral (30 pts)**

Transparency is essential for risk-assessments. This is particularly important for stablecoins, as one of the three functions of money is store of value. If the guarantee, in the form of collateral, is not auditable, then risks cannot be assessed. Hence, this question tries to answer how easy it is to confirm that sufficient collateral is in fact backing the stablecoin.

**Answer:** \
 \
**Score:** 


<table>
  <tr>
   <td><strong>Score</strong>
   </td>
   <td><strong>Description</strong>
   </td>
  </tr>
  <tr>
   <td>30
   </td>
   <td>Independent on-chain verification is possible and easily accessible.
   </td>
  </tr>
  <tr>
   <td>20
   </td>
   <td>Independent verification (also off-chain) is possible, but requires relying on a trusted third-party auditor or reputable entity.
   </td>
  </tr>
  <tr>
   <td>15
   </td>
   <td>On-chain verification is possible but rather complicated.
   </td>
  </tr>
  <tr>
   <td>5
   </td>
   <td>Verification is not possible, but a third-party audit by a reputable audit entity exists
   </td>
  </tr>
  <tr>
   <td>0
   </td>
   <td>Verification is not possible, and no audits exist
   </td>
  </tr>
</table>





# **5. Technical Security - 150 pts**


## This section aims to identify a protocol's security measures that are put in place to prevent hacks, exploits, or uncover other vulnerabilities.

**5.1 Smart Contract Audits (50 pts)**


## Smart contract audits are one of the most important measures to uncover weaknesses in a protocol's technical core. It’s also essential that these audits were performed by firms with a good reputation.


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
   <td>The protocol has undergone 3-4 audits from reputable firms. The latest audit is not older than 6 months.
   </td>
  </tr>
  <tr>
   <td>35
   </td>
   <td>The protocol has undergone 2-3 audits from reputable firms. The latest audit is not older than 12 months.
   </td>
  </tr>
  <tr>
   <td>20
   </td>
   <td>The protocol has undergone 1-2 audits from reputable firms. The latest audit is not older than 18 months.
   </td>
  </tr>
  <tr>
   <td>5
   </td>
   <td>The protocol has undergone 1 audit. This audit is not older than 18 months.
   </td>
  </tr>
  <tr>
   <td>0
   </td>
   <td>The protocol is not audited.
   </td>
  </tr>
</table>


**5.2 Bug Bounty Programs (50 pts)**


## Another very useful method to uncover gaps and vulnerabilities is a public bounty program.


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
   <td>Bounty is 10% of TVL, or at least $1M
   </td>
  </tr>
  <tr>
   <td>40
   </td>
   <td>Bounty is 5% of TVL, or at least 500k
   </td>
  </tr>
  <tr>
   <td>30
   </td>
   <td>Bounty is 250k or higher
   </td>
  </tr>
  <tr>
   <td>20
   </td>
   <td>Bounty is 100k or higher
   </td>
  </tr>
  <tr>
   <td>10
   </td>
   <td>Bounty is 50k or higher
   </td>
  </tr>
  <tr>
   <td>0
   </td>
   <td>No bug bounty program offered or its not active
   </td>
  </tr>
</table>


**5.3 Testing (50 pts)**


## Thoroughly testing a protocol's functionality can help to improve it on many levels. It also helps to improve security. Formal verification processes can further strengthen confidence in a protocol's security.


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
   <td>Protocol has been tested. Testing covered 100% of the protocol. Results are public and a formal verification process was done.
   </td>
  </tr>
  <tr>
   <td>40
   </td>
   <td>Protocol has been tested. Testing covered 75% of the protocol. Results are public and a formal verification process was done.
   </td>
  </tr>
  <tr>
   <td>30
   </td>
   <td>Protocol has been tested. Testing covered 50% of the protocol. Results are public. No formal verification process was done.
   </td>
  </tr>
  <tr>
   <td>20
   </td>
   <td>Some tests are evident, but testing was not complete. No formal verification process
   </td>
  </tr>
  <tr>
   <td>10
   </td>
   <td>No testing, but code was forked.
   </td>
  </tr>
  <tr>
   <td>0
   </td>
   <td>No testing.
   </td>
  </tr>
</table>


**5.6 Penalty for Hacks/Exploits (-300 pts)**


## This section will give minus-points, in case the protocol has previously suffered from hacks or exploits.


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
   <td>-300
   </td>
   <td>Protocol has suffered multiple hacks (2-3) and lost a significant amount of user funds.
   </td>
  </tr>
  <tr>
   <td>-150
   </td>
   <td>Protocol has suffered an exploit and lost a significant amount of user funds.
   </td>
  </tr>
  <tr>
   <td>-50
   </td>
   <td>Protocol has suffered a hack or exploit, but with low impact on user funds.
   </td>
  </tr>
  <tr>
   <td>-25
   </td>
   <td>Protocol has suffered a hack or exploit, but with very little/no impact on user funds.
   </td>
  </tr>
</table>



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
   <td>Fractional- algorithmic
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

