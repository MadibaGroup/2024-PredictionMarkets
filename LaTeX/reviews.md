# Response to Reviewers



## 2026 Financial Cryptography

> **Review #111A**
>
> DePM is one of the critical applications in the blockchain ecosystem. This paper conducts a comprehensive study on DePMs from various perspectives along their lifecycles, including underlying infrastructure, market topic, share structure and pricing, trading, market resolution, settlement, and archiving.

> **Comments for authors:**

> I think this paper is very interesting and I like the topic it discusses. However, I think there are two major issues that should be addressed.

> On the one hand, the quality of the writing and the structure of the paper appear very informal in some sections, especially in Section 3.4, 3.5, and 3.6. For example, in the "The first trade" part of Section 3.4, how to perform splitting and merging is unclear, which directly leads to some of the following sections being incomprehensible. I recommend giving a clear explanation for each definition first, and then using examples to make it easier for readers to understand, rather than just giving an example directly, which would make it more difficult for readers to understand. 

Added formal definitions of each

> This problem also occurs in the "Trading in established markets" part. 

Same as above

> As for Section 3.5, I think the first paragraph should state what market resolution approaches are and be consistent with the subheadings below. 

Changed not exactly as suggested, but addresses this confusion

> For example, the "oracle-less approaches" in the subheading is not mentioned in the first paragraph. As for "A DePM will probably use a hybrid or chained approach that does not rely on a single method...", I think it should be discussed at the end of Section 3.5. 

See above

> Additionally, how many settlement approaches exist? I cannot get this point from Section 3.6.

See above

> On the other hand, in my perspective, the discussion of implications and future research directions is too superficial for a SoK. As a SoK, rather than a survey or literature review, it should provide readers with deeper insights and implications. However, the discussions of composability and regulation in Section 4 currently lack meaningful insights and implications. 

Added a new section on why this fits the definition of an SoK based on 5 previous SoKs. Adjusted the discussion sections.

> Furthermore, the research gaps identified in the "Research Agenda" are quite superficial and arbitrary. 

Reworked and called out research problems so they can be better judged

> I believe that in a SoK, papers should at least partially demonstrate their claims through quantitative experiments. However, the current presentations seem to be ad-hoc, lacking any support.

This is an opinion we do not agree with. We backed our position new paragraph. 

> Except for the above major concerns, here are some minor ones.

> When first mentioning WTA in Section 2.3, the full name should be given.

Fixed

> I am quite confused the definition of "Issuance and Solvency". I think a proper motivating example should be given before introducing this term.

Fixed 

> Table 3 should be explicitly mentioned in this paper.

Fixed

> **Suggested improvements for Revision:** Please refer to my major concerns listed above.

> **Overall merit:** 2. Weak reject

> **Reviewer expertise:** 3. Knowledgeable



> **Review #111B**
>
> *Paper summary:** This SoK paper discusses the market microstructure of decentralized prediction markets. It discusses technical building blocks, market functions, etc. and identifies open problems for further research.
>
> **Comments for authors:** 
>
> Strengths:
>
> * Prediction markets are an interesting topic and certainly relevant for FC. A good SoK paper would be beneficial for the community.

> Weaknesses:
>
> - In its current state, the article doesn't provide much added value beyond a simple literature review. It doesn't provide any novel insights or challenge commonly held assumptions

Added section talking about what SoKs generally do and why our paper fits the history of SoKs at FC and AFT in recent years

- > At the end, the paper brings up some research questions but they are not derived from some deeper reflection on research gaps.

Tried to enhance the future research and made it more prominent

- > It lacks scientific rigour and suffers from quality issues (see notes below)

Punt on rigour, is consistent with other SoKs on rigour. Quality addressed below. 

> **Notes and Specific Comments:**
>
> Abstract:
>
> - Also for a SoK paper there should be some overarching questions and specific contributions, which should be reflected in the abstract.

I disagree about overarching questions, it is a way to do an SoK but not a requirement. The specific contribution is the modular framework

> Introduction:
>
> - I miss a clear explanation of the underlying motivation, specific objectives and contributions of this SoK.
> - The current overarching question "what are the design decisions..." is too broad and doesn't reflect the title

Tried to enhance

> Preliminaries
>
> - I miss an explanation of the applied systematization methodology; it should go beyond collecting a list of relevant papers

Enhanced methodology section

> - How did the authors come up with this specific taxonomy?

Enhanced methodology section

> - I don't see the need for formal definitions here; especially since this is supposed to be a SoK paper; I'd rather expect a simple description of how prediction markets work

This is an opinion. Others will have the opposite opinion. Consensus: keep unless if it becomes a recurring theme from reviewers

> Modular Workflow
>
> - What is the underlying motivation for this exact workflow? Is it based on previous literature, has it been derived from some other form of evidence? Also, the figure misses a caption.

Moved methodology, replaced visualization with just textual description

- > The title of subsection 3.2 "market topic" is somehow misleading because the following text discusses permission models

It is meant to discuss both, can think if we can make it clearer

- > It remains unclear how the authors found these pitfall examples

Addressed in new methodology section

- > The share structure and pricing subsection is somehow interesting. It could be improved by, for instance, a table mapping specific markets to these categories and discussing possible nuances.

If by specific markets, they mean specific DePMs, our table later addresses this. We also give lots of examples of each kind within Polymarket

- > The same holds for the subsequent subsections. I somehow miss the systematization aspect there

Not clear what to do, leaving aside

> **Discussion:** The discussion points seem somehow arbitrary; I'd expect some reflection on findings and a deeper reflection of possible research directions.
>
> **Overall merit:** 1. Reject
>
> **Reviewer expertise:** 3. Knowledgeable



## 2026 WTSC

> **Review 1**
> Overall evaluation	
> 2: accept
> SoK: Market Microstructure for Decentralized Prediction Markets (DePMs).
>
> I found this a good summary of prediction markets. It began with Polymarket's famous prediction, which was a good start. It had a lot of good theory. There was, however, no definition or linkage to the term Microstructure, as used in the title.

Good point, added.

> There was some angst expressed about it being an SoK (its "difficult to establish what constitutes an SoK paper.") There were research gaps identified, which is more statement of lack of knowledge. That is fine, but they were not well incorporated into the text and offered no insight as to how to evaluate research on those outstanding issues.



> The conclusion looked like an afterthought. I could be more comprehensive.



> I recommend accept but think the minor issues above could be addressed for the publication of the conference proceedings.



> **Review 2**
> Overall evaluation	
> 3: strong accept
> I think the paper is a very well done survey on Decentralised Prediction Markets, an important type of market which is gaining traction over the last few years.



> **Review 3**
> Overall evaluation	
> 2: accept
> Summary
> The paper discusses the various designs of DePMs, utilizing a modular workflow specifically designed for this purpose. It presents a systems-thinking approach to DePMS, covering the technical substrate (infrastructure), the economic primitives (share structure/pricing), and the functional lifecycle (initialization, trading, resolution, settlement, archiving). Using an effective framework to compare DePM designs, the authors arrive at a comprehensive SoK, which is structurally sound, historically faithful, well-written, detailed, and precise.
>
> The references include numerous recent publications.
> It includes informative appendices.



> Some minor changes would improve the paper:
> 2.2 Definitions:
>
> Definition 1: Arrow-Debreu instead of Arrow--Debreu



> Definition 2:
> prediction market instead of prediction-market
> (unit of accounting) instead of (unit of account)
> res(M) is not a function if it may return two different values for the same M. Consider adding something like time as an additional parameter (probably from a discrete range, say t \in N), writing it as res_t(M) or res(M,t). Then you can characterise the admissible functions as res_t(M) = \bot for t < t_0 and = \omega for t >= t_0, for some fixed t_0 and \omega. As t_0 and \omega are fixed per market, you might as well add t_0 and \omega to the definition of the market, making it a 5-tuple. Then, res(M) doesn't need an additional parameter, as its result depends solely on the components of M.



> Definition 3:
>
> 1. bad notation, S looks like \mathcal S.
>   Define what you mean by "outstanding supplies". This notion is hardly used throughout the paper and hasn't been introduced yet. Moreover, the phrase "outstanding supply vector" is hard to parse (as "outstanding" often means excellent/exceptional). Consider rewriting it to "vector of outstanding supplies".
> 2. per-label instead of per--label
>   Out of the blue, you mention holdings and accounts. It may be clearer if you first introduce the notion of an abstract fungible token with the associated and familiar notions of accounts, transfers, burning, and creation, and then specify that J is a finite set of such tokens. Saying that J is just a set of labels is less abstract than it seems, since you implicitly assume that each label has the properties of a fungible token.
> 3. This condition becomes less obfuscated if time and t_0 are introduced explicitly, as it becomes "If t >= t_0, any holder may redeem".
>



> 3 Modular Workflow
> Why is this a workflow? Is there a temporal order? Or is it rather a collection of 8 categories or dimensions, along which you classify DePMs?



> 3.3 eq (4):
> The mathematical typography is confusing. Usually, we use (math-)italic letters for variables (including names for functions that are not fixed), and upright letters for constants with a fixed meaning. It seems that you use a sans-serif font for the latter. Why is k sans-serif, if it is just a place-holder for an arbitrary value (a.k.a. a variable)? Similarly, it is not quite clear why res is upright, when it is actually a placeholder (and thus should be \mathit{res}), and L is italic, when it is actually an operator with a fixed meaning.



> References 29 and 53 are missing source information.
> Thorough proofreading would be nice.



> Suggestion for future applications:
> Even though no major DePM protocol yet implements an end-to-end autonomous feedback loop, you may want to include it in your last stage (thereby going beyond preservation). Learning loops already exist in some systems, but they are still fragmented and not fully automated.
