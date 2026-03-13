| Symbol                                | Brief description                                            | Introduced                                            | Symbol type                | Typical notation?                                            |
| ------------------------------------- | ------------------------------------------------------------ | ----------------------------------------------------- | -------------------------- | ------------------------------------------------------------ |
| \(M\)                                 | A single market instance                                     | Def. 1 (Market)                                       | structured object (tuple)  | ✓                                                            |
| \(\Omega\)                            | Outcome space for \(M\) (set of possible resolutions)        | Def. 1 (Market)                                       | set                        | ✓                                                            |
| \(J\)                                 | Index set of fungible token types (share-token types)        | Def. 1 (Market)                                       | finite index set           | ✓                                                            |
| \(R:\Omega\to\mathbb{R}_{\ge 0}^{J}\) | Payoff map; \(R(\omega)_j\) is payout (in \(\mathcal N\)) per unit of token type \(j\) if outcome is \(\omega\) | Def. 1 (Market)                                       | map / function             | ✓ *(often italic; upright also OK if you declare a convention)* |
| \(t_{\mathrm{res}}\in\mathbb{N}\)     | Scheduled resolution time (discrete)                         | Def. 1 (Market)                                       | variable / parameter       | ✓ *(roman subscript is standard)*                            |
| \(\mathbb{N}\)                        | Discrete time domain (natural numbers)                       | Def. 1 (Market)                                       | set                        | ✓                                                            |
| \(\mathbb{R}_{\ge 0}^{J}\)            | Nonnegative real vectors indexed by \(J\)                    | Def. 1 (Market)                                       | set / vector space         | ✓                                                            |
| \(\iota:J\to\Omega\)                  | Bijection associating each token type \(j\in J\) with a unique outcome in \(\Omega\) | Remark (WTA special-case)                             | bijection (map)            | ✓                                                            |
| \(\omega\)                            | Outcome variable (element of \(\Omega\))                     | Remark (WTA special-case)                             | variable (element)         | ✓                                                            |
| \(j\)                                 | Token type index (element of \(J\))                          | Remark (WTA special-case) *(also implicit in Def. 1)* | variable (index/element)   | ✓                                                            |
| \(\{0,1\}\)                           | Binary payoff range for WTA tokens                           | Remark (WTA special-case)                             | set                        | ✓                                                            |
| \(\sum_{j\in J} R(\omega)_j = 1\)     | Completeness condition for WTA payoffs (total payout across all WTA tokens is 1 for any \(\omega\)) | Remark (WTA special-case)                             | constraint / property      | ✓                                                            |
| WTA                                   | Winner-take-all market type                                  | Remark (WTA special-case)                             | terminology / market class | ✓                                                            |
| Arrow–Debreu                          | Contingent-claim synonym for WTA structure                   | Remark (WTA special-case)                             | terminology / market class | ✓                                                            |
| \(\mathcal{S}\)        | Prediction market system                                     | Def. 2 (Prediction Market System) | structured object (tuple)       | ✓                                                  |
| \(\mathcal{M}\)        | Countable set of markets                                     | Def. 2                            | set                             | ✓                                                  |
| \(\mathcal{N}\)        | Numeraire (unit of accounting)                               | Def. 2                            | unit / symbol for currency      | ✓                                                  |
| \(\mathrm{res}(M,t)\)  | Resolution function value at discrete time \(t\); either unresolved \(\bot\) or final outcome \(\omega\in\Omega\) | Def. 2                            | function                        | ✓ *(upright is standard for fixed operator names)* |
| \(t\in\mathbb{N}\)     | Discrete time variable                                       | Def. 2                            | variable (index)                | ✓                                                  |
| \(\bot\)               | “Unresolved” marker for resolution                           | Def. 2                            | constant / distinguished symbol | ✓                                                  |
| \(t_{\mathrm{res}}\)   | Scheduled resolution time for market \(M\)                   | Def. 2 *(also Def. 1)*            | parameter (integer)             | ✓                                                  |
| \(\{\bot\}\cup\Omega\) | Codomain of \(\mathrm{res}(M,t)\) for a fixed market         | Def. 2                            | set                             | ✓                                                  |
| \(\omega\)             | Final realized outcome (element of \(\Omega\))               | Def. 2 *(also WTA remark)*        | variable / element              | ✓                                                  |
| \(\mathsf{Treas}_M\)                          | Treasury associated with market \(M\) (in \(\mathcal N\))    | Def. 3 (System Axioms) | state variable / quantity   | ✓                                                            |
| \(\mathsf{Treas}:=\mathsf{Treas}_M\)          | Abbreviation for the fixed market’s treasury inside Def. 3   | Def. 3                 | definitional abbreviation   | ✓                                                            |
| \(Q=(Q_j)_{j\in J}\in\mathbb{R}_{\ge 0}^{J}\) | Vector of outstanding token supplies (issued minus burned)   | Def. 3, Axiom 1        | vector / state variable     | ✓                                                            |
| \(Q_j\)                                       | System-wide outstanding supply (total units) of token type \(j\) | Def. 3, Axiom 1        | scalar (component of \(Q\)) | ✓                                                            |
| \(\mathrm{L}(Q)\)                             | Worst-case liability functional \(\sup_{\omega}\sum_j Q_jR(\omega)_j\) | Def. 3, Axiom 1        | operator / functional       | ✓                                                            |
| \(\mathrm{L}:=\mathrm{L}_M\)                  | Abbreviation for the fixed market’s liability functional     | Def. 3 (preamble)      | definitional abbreviation   | ✓ *(but note: your text currently says \(L:=L_M\); should match \(\mathrm{L}\))* |
| \(Q'\)                                        | Updated outstanding-supply vector after an operation         | Def. 3, Axiom 1        | variable (post-state)       | ✓                                                            |
| \(\Delta \mathsf{Treas}\)                     | Change in treasury due to an operation                       | Def. 3, Axiom 1        | variable (delta)            | ✓                                                            |
| \(a\ge 0\)                                    | Amount of token units held/redeemed by an account            | Def. 3, Axiom 2–3      | variable (scalar)           | ✓                                                            |
| \(t\ge t_{\mathrm{res}}\)                     | “After resolution time” condition enabling redemption        | Def. 3, Axiom 3        | condition / inequality      | ✓                                                            |





| Symbol                                             | Brief description                                            | Introduced           | Symbol type                    | Typical notation?                                            |
| -------------------------------------------------- | ------------------------------------------------------------ | -------------------- | ------------------------------ | ------------------------------------------------------------ |
| \(\mathsf{A},\mathsf{B},\mathsf{C}\)               | Named example outcomes (elements of \(\Omega\))              | Sec. 3.3 WTA example | constants (example outcomes)   | ✓ *(upright/sans-serif for named states is common; italic also fine)* |
| \(j_{\mathsf{A}}, j_{\mathsf{B}}, j_{\mathsf{C}}\) | Token types corresponding to the example outcomes            | Sec. 3.3 WTA example | identifiers / token-type names | ✓                                                            |
| \(k\in\{\mathsf{A},\mathsf{B},\mathsf{C}\}\)       | Bound variable ranging over the example outcomes             | Sec. 3.3 WTA example | variable (index/element)       | ✓                                                            |
| \(j_{k}\)                                          | Token type corresponding to outcome \(k\) (WTA “claim on \(k\)”) | Sec. 3.3 WTA example | indexed token type             | ✓ *(clear if you state the convention “\(k\mapsto j_k\)”)*   |
| \(R(\omega)_{j_k}\in\{0,1\}\)                      | WTA payoff for token \(j_k\): pays 1 iff \(\omega=k\)        | Sec. 3.3 WTA example | payoff expression / predicate  | ✓                                                            |






| Symbol                                        | Brief description                                            | Introduced   | Symbol type                          | Typical notation?                                            |
| --------------------------------------------- | ------------------------------------------------------------ | ------------ | ------------------------------------ | ------------------------------------------------------------ |
| YNB                                           | Yes-no bundle market structure                               | Sec. 3.3 YNB | terminology / market class           | ✓                                                            |
| \(j_{\mathsf{A_Y}}, j_{\mathsf{A_N}}, \dots\) | Example token types: for each outcome \(\mathsf{A},\mathsf{B},\mathsf{C}\), a YES-token and a NO-token | Sec. 3.3 YNB | identifiers / token-type names       | ✓                                                            |
| \(j_{k_Y}\)                                   | YES token type for outcome \(k\)                             | Sec. 3.3 YNB | indexed token type                   | ✓ *(better as \(j_{k_Y}\) with italic \(k\); avoid \(\mathsf{k}\))* |
| \(j_{k_N}\)                                   | NO token type for outcome \(k\) (“not-\(k\)”)                | Sec. 3.3 YNB | indexed token type                   | ✓ *(same note as above)*                                     |
| \(k_Y, k_N\)                                  | Suffix notation indicating YES/NO variant of outcome \(k\)   | Sec. 3.3 YNB | naming convention                    | ✓                                                            |
| \(R(\omega)_{j_{k_Y}}\)                       | Payoff of YES token: 1 iff \(\omega=k\)                      | Sec. 3.3 YNB | payoff expression                    | ✓                                                            |
| \(R(\omega)_{j_{k_N}}\)                       | Payoff of NO token: 1 iff \(\omega\neq k\)                   | Sec. 3.3 YNB | payoff expression                    | ✓                                                            |
| “not-\(k\)”                                   | Complement event of outcome \(k\) within \(\Omega\)          | Sec. 3.3 YNB | informal notation / event complement | ✓                                                            |



| Symbol                                                       | Brief description                                            | Introduced      | Symbol type                   | Typical notation?                             |
| ------------------------------------------------------------ | ------------------------------------------------------------ | --------------- | ----------------------------- | --------------------------------------------- |
| YNB-NR                                                       | “Negative risk” variant of YNB where YES side is complete and exclusive across \(\Omega\) | Sec. 3.3 YNB-NR | terminology / market class    | ✓                                             |
| \(\lvert\Omega\rvert\)                                       | Number of outcomes in \(\Omega\)                             | Sec. 3.3 YNB-NR | cardinality                   | ✓                                             |
| \(\sum_{k\in\Omega} R(\omega)_{j_{k_Y}}=1\)                  | YES-side completeness/exclusivity expressed as “YES payoffs sum to 1” | Sec. 3.3 YNB-NR | constraint / property         | ✓ (use italic \(k\), not \(\mathsf{k}\))      |
| \(\sum_{k\in\Omega} R(\omega)_{j_{k_N}}=\lvert\Omega\rvert-1\) | NO-side total payoff identity in YNB-NR                      | Sec. 3.3 YNB-NR | constraint / derived identity | ✓                                             |
| \(\Omega\setminus\{k\}\)                                     | Outcome set excluding outcome \(k\)                          | Sec. 3.3 YNB-NR | set difference                | ✓                                             |
| \(\ell\)                                                     | Bound variable ranging over outcomes (used in sums)          | Sec. 3.3 YNB-NR | variable (index/element)      | ✓                                             |
| *negRisk*                                                    | Conversion gadget enabling payoff-equivalent portfolio transformations | Sec. 3.3 YNB-NR | mechanism / terminology       | ✓                                             |
| \(R(\omega)_{j_{k_N}}=\sum_{\ell\in\Omega\setminus\{k\}} R(\omega)_{j_{\ell_Y}}\) | NO-to-YES payoff equivalence                                 | Sec. 3.3 YNB-NR | payoff identity               | ✓                                             |
| \(\lvert\Omega\rvert-2\)                                     | Constant cash term appearing in the YES-from-NOs identity    | Sec. 3.3 YNB-NR | scalar constant               | ✓                                             |
| \(A\subseteq\Omega\)                                         | Subset of outcomes used to describe a NO-portfolio over multiple outcomes | Sec. 3.3 YNB-NR | set (subset)                  | ✓                                             |
| \(\lvert A\rvert>0\)                                         | Nonempty subset condition                                    | Sec. 3.3 YNB-NR | condition                     | ✓                                             |
| \(\lvert A\rvert\)                                           | Number of outcomes in \(A\)                                  | Sec. 3.3 YNB-NR | cardinality                   | ✓                                             |
| \(\sum_{k\in A} R(\omega)_{j_{k_N}}=(\lvert A\rvert-1)+\sum_{\ell\in\Omega\setminus A} R(\omega)_{j_{\ell_Y}}\) | “Cash extraction” identity for NO-portfolio over \(A\) outcomes | Sec. 3.3 YNB-NR | payoff identity               | ✓ (ensure the quantifier says nonempty \(A\)) |



| Symbol                           | Brief description                                            | Introduced              | Symbol type                      | Typical notation?                 |
| -------------------------------- | ------------------------------------------------------------ | ----------------------- | -------------------------------- | --------------------------------- |
| \(X:\Omega\to\mathbb{R}\)        | Observed scalar quantity associated with each outcome \(\omega\) (e.g., temperature, vote share) | App. A (Scalar Markets) | map / function                   | ✓                                 |
| \(\mathbb{R}\)                   | Real numbers (codomain of \(X\))                             | App. A                  | set                              | ✓                                 |
| \([a,b]\)                        | Lower/upper bounds used to cap and normalize the scalar quantity | App. A                  | interval (set)                   | ✓                                 |
| \(a,b\)                          | Lower and upper bound parameters                             | App. A                  | parameters (scalars)             | ✓                                 |
| \(j_{\mathrm{lin}}\)             | Linear/scalar token type (the “linear outcome share”)        | App. A                  | token type identifier            | ✓ *(roman subscript is standard)* |
| \(R(\omega)_{j_{\mathrm{lin}}}\) | Payout of the linear token at outcome \(\omega\), normalized to \([0,1]\) with caps at \(a,b\) | App. A                  | payoff expression                | ✓                                 |
| \(X(\omega)\)                    | Realized value of the scalar quantity under outcome \(\omega\) | App. A                  | expression (function evaluation) | ✓                                 |
| \(b-a\)                          | Normalization denominator (range width)                      | App. A                  | scalar expression                | ✓                                 |



| Symbol                                  | Brief description                                            | Introduced                  | Symbol type                | Typical notation?                                            |
| --------------------------------------- | ------------------------------------------------------------ | --------------------------- | -------------------------- | ------------------------------------------------------------ |
| \(\mathsf{Treas}\in\mathbb{R}_{\ge 0}\) | Loss fund / treasury posted by the automated bookmaker (in \(\mathcal N\)) | Def. (Automated bookmaking) | state variable / quantity  | ✓ *(already used in Def. 3; here it is re-used as the bookmaker’s fund)* |
| “pricing rule (odds)”                   | Rule that determines quoted prices for token types \(j\in J\) | Def. (Automated bookmaking) | mechanism component (rule) | ✓                                                            |
| \(S\)                                   | Supply vector updated by issuance during bookmaking          | Def. (Automated bookmaking) | vector / state variable    | ⚠︎ *(inconsistent with earlier choice \(Q\); also looks like \(\mathcal S\))* |



| Symbol                                        | Brief description                                            | Introduced                   | Symbol type                 | Typical notation? |
| --------------------------------------------- | ------------------------------------------------------------ | ---------------------------- | --------------------------- | ----------------- |
| \(B\)                                         | Unit bundle: a fixed set of WTA token types that together have constant payoff 1 | Def. (Splitting and merging) | set (bundle of token types) | ✓                 |
| \(\sum_{j\in B} R(\omega)_j = 1\)             | Bundle payoff condition: the bundle pays 1 unit of numeraire for any outcome \(\omega\) | Def. (Splitting and merging) | constraint / property       | ✓                 |
| \(1\cdot\mathcal{N}\mapsto \sum_{j\in B} j\)  | Splitting operation: exchange 1 unit of numeraire for one unit of each token in \(B\) | Def. (Splitting and merging) | state transition / mapping  | ✓                 |
| \(\sum_{j\in B} j \mapsto 1\cdot\mathcal{N}\) | Merging operation: exchange the bundle for 1 unit of numeraire | Def. (Splitting and merging) | state transition / mapping  | ✓                 |
| “unit bundle”                                 | Bundle containing one unit of each token type in \(B\)       | Def. (Splitting and merging) | terminology                 | ✓                 |