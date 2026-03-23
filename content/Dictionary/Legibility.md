---
type: term
domain:
  - AI Ethics
  - Political Science
  - UX Design
status: seed
aliases:
  - Systemic Readability
  - Explainability
  - XAI
related:
  - [[Trustworthy UX]]
  - [[Black-box Theology]]
  - [[Teleological Interface]]
sources:
  - James C. Scott
  - Frank Pasquale
  - 1 John 1
---

## Definition
The ethical mandate that any technological or bureaucratic system holding power over a human being must be understandable ("readable") by that human. It asserts that if a system can judge you, influence you, or restrict you, you have a moral right to know *how* it works.

Derived from James C. Scott’s work, "Legibility" originally described how states simplify society to control it (maps, surnames, grids). In the AI era, the power dynamic has flipped: systems are now so complex ("Black Boxes") that they are illegible to the humans they govern.

**Legibility as a Moral Minimum** argues that "transparency" (dumping raw code) is not enough. The system must be *comprehensible*. If an AI denies your loan, curates your news, or flags your account, and it cannot explain *why* in plain language, it is operating below the moral minimum of human dignity. You cannot consent to a system you cannot read.

## Signs / markers

- **"Why am I seeing this?" Features:** Buttons on ads or feeds that reveal the specific data points targeting you.
    
- **Plain Language Explanations:** Terms of Service that use simple summaries alongside the legalese (e.g., "We sell your location data" vs. "We share telemetry with third-party partners").
    
- **Recourse Mechanisms:** The ability to not just _see_ the logic, but _challenge_ it (e.g., "This data point about me is wrong; correct it").
    

## Examples (culture / tech / daily life)

- **Credit Score Reports:** One of the few "Legible" algorithms. You are told exactly why your score went down (e.g., "High credit utilization"), allowing you to change your behavior.
    
- **The TikTok Algorithm (Illegible):** You do not know why a specific video is shown to you. Is it because you liked a cat video 3 weeks ago? Or because the creator paid for reach? The opacity prevents you from auditing your own formation.
    
- **Kafka’s "The Trial":** The ultimate story of **Illegibility**. The protagonist is arrested and tried but never told the charge. This is the nightmare scenario of modern AI bureaucracy.
    

## Contrasts

- **Opposite:** [[Black Box]] (A system where inputs and outputs are visible, but the logic is hidden).
    
- **Related-but-not-the-same:** [[Transparency]] (Transparency is showing the data; Legibility is making the data _understandable_. A dump of 10 million lines of code is transparent but illegible).
    

## Related terms

- [[Trustworthy UX]]
    
- [[Digital Discernment]] (Discernment is impossible without Legibility).
    
- [[Algorithmic Formation]]
    

## Biblical lens (NKJV)

**Scripture:** > "This is the message which we have heard from Him and declare to you, that God is light and in Him is no darkness at all." (1 John 1:5, NKJV)

**Discernment:** Darkness is the domain of confusion and hidden agendas. Light is the domain of truth and revelation. A "Godly" system brings things into the light—it reveals truth. A demonic system operates in obscurity, keeping people confused about their standing and their reality. We are called to be "Children of Light" (Ephesians 5:8), which implies we should build systems that do not hide their mechanisms.

## Sources / lineage

- **Political Theory:** *[Seeing Like a State (James C. Scott)](http://kokolabs.org/Scott%20-%20Seeing%20Like%20a%20State%20(Intro,%20cp%201-3).pdf)* — *The origin of the term "legibility," analyzing how high-modernist states simplify complex societies to control them.*

- **Legal Theory:** *[The Black Box Society (Frank Pasquale)](https://raley.english.ucsb.edu/wp-content/Engl800/Pasquale-blackbox.pdf)* — *A seminal text arguing that authority is increasingly expressed through secret algorithms, necessitating a "intelligible society."*

- **Regulatory Framework:** *[GDPR Article 22 (EU Legislation)](https://ejlt.org/index.php/ejlt/article/download/570/772/2774#:~:text=Article%2022%20GDPR%20bans%20all,safeguards%20for%20data%20subject%20rights.)* — *The legal attempt to codify a "Right to Explanation" regarding automated decision-making.*

## Notes
- **The "Consent" Argument:** Meaningful consent is impossible without Legibility. If the user doesn't understand the trade-off, they didn't actually agree to it.

## Diagram

```mermaid
flowchart TD
    %% Global Graph Settings
    %% This adds space between the two subgraphs
    
    subgraph S1 ["The Illegible System (Black Box)"]
        A1[Human User] -->|Inputs Data| B1("AI / Bureaucracy<br/>Black Box")
        B1 -->|Judgement/Restriction| C1[Human User]
        C1 --"Why?"--> D1{"???<br/>Trade Secret"}
        D1 -->|Result| E1["Confusion &<br/>Loss of Agency"]
        
        %% Styling for White Text on Dark Background
        style B1 fill:#333,stroke:#666,color:#fff
        style D1 fill:#555,stroke:#777,color:#fff
    end

    %% Invisible strut to force spacing between S1 and S2
    E1 ~~~ S2

    subgraph S2 ["The Legible System (Moral Minimum)"]
        A2[Human User] -->|Inputs Data| B2("AI / Bureaucracy<br/>Transparent")
        B2 -->|Judgement/Restriction| C2[Human User]
        C2 --"Why?"--> D2["Plain Language Explanation<br/>& Recourse Mechanism"]
        D2 -->|Result| E2["Understanding &<br/>Consent"]
        
        %% Styling for Legible System
        style B2 fill:#e6f7ff,stroke:#1890ff,color:#000
        style D2 fill:#d9f7be,stroke:#52c41a,color:#000
    end
