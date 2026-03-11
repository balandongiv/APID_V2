# Overview

This planning document outlines how to enrich the APID hydroponics tutorial handbook with pedagogical `tcolorbox` blocks. Each box will reinforce learning, warn about pitfalls, or bridge the current session with upcoming material. The handbook comprises twelve main sessions (Session 1 through Session 12) plus an introductory set of materials. Sessions 5 and 6 are combined in a single LaTeX file but are treated here as two distinct activities (individual work and group consolidation) for planning purposes. The narrative traces a complete product-development cycle: from identifying an opportunity, through planning, needs analysis and specification, to concept generation, selection, and testing. The tone throughout the handbook is instructional and pragmatic, with a focus on hydroponic applications and applied physics.

The refactoring goal is to insert `tcolorbox` environments using the template:

```latex
\begin{tcolorbox}[title=]
...
\end{tcolorbox}
```

Boxes may be labelled **Goal**, **Checkpoint**, **Common Mistakes** or **Hint** depending on their purpose. Their content should be concise and closely related to the surrounding material, and they should help learners navigate the chapter, verify their progress, avoid frequent pitfalls, or provide helpful prompts. Wherever possible, boxes anticipate upcoming sessions or echo earlier decisions to build continuity across the handbook. Citations in brackets refer to the relevant portions of the existing LaTeX text, for later reference by the editing specialist.

# Global Observations

* **Pedagogical structure:** Each session opens with a clear overview and learning objectives, followed by definitions, pre-class and in-class activities, templates and tables, and a summary. The prose is formal, but plain enough for undergraduate readers. Many sessions explicitly connect to earlier work: for example, Session 4 builds on the innovation charter of Session 3, and Session 7 draws upon the mission statement from Sessions 5 and 6.

* **Opportunity for scaffolding:** Learners are asked to make decisions in steps—first choosing a product and company, later selecting a development process, drafting an innovation charter, generating and screening opportunities, analysing markets, specifying needs and metrics, decomposing functions, generating concepts, selecting concepts, and testing them. Placing **Goal** boxes near the start of each chapter will summarise these objectives and set expectations.

* **Frequent pitfalls:** The sessions caution against overly narrow charters, ideas that drift away from hydroponics, confusing process type with organisational structure, jumping to solutions too early, or relying on unverified LLM outputs. **Common Mistakes** boxes can make these warnings explicit.

* **Verification points:** Many activities require tangible outputs—selecting a product, generating at least five opportunities, completing market analysis tables, assigning importance scores, etc. These are natural locations for **Checkpoint** boxes to remind students what to produce before moving on.

* **Hints for continuity:** Because each chapter builds on previous decisions, **Hint** boxes can encourage students to revisit earlier outputs (for example, using the innovation charter when generating opportunities or using needs and metrics when selecting concepts).

The following session-by-session plan proposes specific insertion points, draft box content, rationales, and links to previous and upcoming chapters. Each insertion is listed with a status checkbox to aid the later editing specialist.

# Session-by-Session Plan

## Session 1 – Opportunity Identification in Hydroponic Agriculture

**Summary:** Introduces the project and asks each group to identify a realistic product opportunity within hydroponic agriculture, then place it within a believable company context. Key sections define what counts as a direct or indirect hydroponic product, provide example opportunity areas, list evaluation criteria, and outline activities for selecting the product and company.

### Proposed insertions

* [ ] **Goal** after the learning objectives (after L18).
  **Draft content:** “Summarise today’s mission: identify a specific hydroponic product opportunity and select a plausible company context. Focus on opportunities that solve a meaningful hydroponics problem, provide enough technical depth for later physics analysis, and fit within your team’s capability.”
  **Rationale:** Clarifies what success looks like for this session and reminds students of the two-fold decision they must make.
  **Continuity:** Links forward to development strategy (Session 2) and market analysis (Sessions 5 & 6).

* [ ] **Common Mistakes** near the “What Counts as a Suitable Product?” section (around L36).
  **Draft content:** “Avoid generic or loosely related ideas. Your product must have a clear and defensible connection to hydroponics and enough technical depth for applied physics work. Don’t choose an idea simply because it seems trendy; evaluate need, feasibility, user impact, physics relevance and team capability.”
  **Rationale:** Warns against superficial or off-topic ideas.
  **Continuity:** Prepares students for Session 2’s process selection and Session 3’s charter definition.

* [ ] **Hint** before Activity 1.
  **Draft content:** “Brainstorm both direct products (e.g., nutrient mixers, pumps, monitoring sensors) and indirect products (e.g., maintenance tools, storage units). If you struggle to decide, conduct a quick market scan to see what products already exist and how yours might be differentiated.”
  **Rationale:** Encourages a broad search before narrowing down to one idea.

* [ ] **Checkpoint** just after the “Expected Output” bullet list (around L88).
  **Draft content:** “Before moving on, ensure that your team has:

  * selected a product;
  * stated the specific hydroponics problem it solves; and
  * documented why this idea was preferred over other candidates.
    Capture this in point form to upload to ITEL.”
    **Rationale:** Ensures completion of the deliverables before starting company selection and prevents progress without a clear outcome.
    **Continuity:** This summary feeds directly into Sessions 2 and 5.

* [ ] **Checkpoint** after “Activity 2: Select the Company Context” (around L97–L123).
  **Draft content:** “Confirm your chosen company type (established vs. start-up) and record your reasoning with respect to target users, resources, quality level, market position and price strategy. This context will influence manufacturing and market analysis later.”
  **Rationale:** Encourages explicit documentation of company assumptions, which will be used in market planning (Sessions 5 & 6).

---

## Session 2 – Stage-Gate and Development Strategy

**Summary:** Guides teams to decide how work will be organised and reviewed through the project. Students must select a development process type, choose a process flow (generic, spiral, complex-system), identify required departments and organisational structures, and justify their choices.

### Proposed insertions

* [ ] **Goal** after the learning objectives (after L19).
  **Draft content:** “Today you will choose the process and structure for your project. Identify a suitable product-development process (market-pull, technology-push, etc.), select a flow pattern (linear, spiral, or complex-system), determine which departments must contribute, and propose an organisational structure.”
  **Rationale:** Summarises the four decisions the team must make and clarifies their importance.

* [ ] **Common Mistakes** after the Key Terms section (around L37–L53).
  **Draft content:** “Don’t confuse a development process type (e.g., market-pull) with a process flow (e.g., spiral). Remember that departmental structure (who participates) is different from organisational structure (how authority is arranged). Avoid picking a process without considering product complexity and uncertainty.”
  **Rationale:** Addresses common conceptual confusions.

* [ ] **Hint** beside the Product Development Process Flows section (around L65–L88).
  **Draft content:** “Match the process flow to your product’s technical uncertainty and subsystem interactions. Use a generic flow for low-risk projects, a spiral flow when iteration is essential, and a complex-system flow if multiple subsystems must be integrated. Consider that electronics, fluid handling and structure often benefit from a spiral or complex approach.”
  **Rationale:** Encourages thoughtful selection rather than defaulting to a generic flow.

* [ ] **Checkpoint** after the Pre-Class Preparation instructions (around L133–L147).
  **Draft content:** “Each member should prepare notes on:

  1. the most suitable development process type;
  2. the most suitable development process flow;
  3. essential departments; and
  4. the recommended organisational structure, with a short justification.
     Verify that all four decisions are addressed before class.”
     **Rationale:** Ensures students come prepared and avoids shallow discussion during class.

---

## Session 3 – Innovation Charter and Opportunity Identification

**Summary:** Explains the purpose of an innovation charter, provides examples of good charter statements, and guides students through drafting, evaluating and selecting a final charter. It emphasises breadth, relevance, feasibility, physics connection and potential impact.

### Proposed insertions

* [ ] **Goal** after the objectives list (after L19).
  **Draft content:** “Your task today is to draft and agree on an innovation charter for your project. A good charter identifies the problem area, product category, target users and time frame, stays within the hydroponics theme, leaves room for multiple opportunities, supports applied-physics analysis, and remains achievable.”
  **Rationale:** Consolidates the characteristics of a strong charter.

* [ ] **Common Mistakes** next to the “Drafting Guidance” subsection (around L68–L79).
  **Draft content:** “Avoid writing a charter that already specifies the exact mechanism, geometry or final concept—such statements are too narrow. Equally, avoid vague goals like ‘make hydroponics better’; include the product category, target market and time frame.”
  **Rationale:** Prevents extremes of over-specificity and vagueness.

* [ ] **Hint** below the example charters (around L49–L59).
  **Draft content:** “Notice how the sample charters identify a category (e.g., compact hydroponic support product), the intended users (small-scale growers) and a time frame (one academic semester). Use this pattern as inspiration when drafting your own statements.”
  **Rationale:** Gives a model to emulate.

* [ ] **Checkpoint** at the end of the Pre-Class Activity instructions (after L90).
  **Draft content:** “Ensure you bring at least two draft charters to class, each accompanied by a one-line note explaining why it is promising. Without these drafts the in-class comparison cannot proceed.”
  **Rationale:** Promotes accountability.

* [ ] **Checkpoint** after the In-Class Activity instructions (around L119–L127).
  **Draft content:** “Once the discussion concludes, write the final charter agreed by the team, ensure it meets the relevance, breadth, feasibility, physics connection and impact criteria, and record the rationale for its selection.”
  **Rationale:** Ensures a documented final statement for use in Session 4.

---

## Session 4 – Opportunity Identification

**Summary:** Uses the innovation charter to generate multiple opportunity options, record them using a structured template, and screen them using criteria such as alignment, impact, feasibility, technical depth and resource fit.

### Proposed insertions

* [ ] **Goal** after the overview (after L20).
  **Draft content:** “In this session, convert your innovation charter into several concrete opportunities. Generate at least five options that fit the charter, describe how each could create value for hydroponic users, and prepare to screen them using objective criteria.”
  **Rationale:** Focuses attention on breadth of idea generation and systematic screening.

* [ ] **Hint** within the “How to Brainstorm” list (around L58–L70).
  **Draft content:** “Refer back to your innovation charter to stay within scope. Think beyond obvious product improvements—consider user frustrations, technical issues (flow, sensing, maintenance, energy), safety, efficiency, reliability, usability, and emerging technologies. Document each opportunity with a clear description and its relationship to the charter.”
  **Rationale:** Provides concrete prompts for idea generation.

* [ ] **Checkpoint** just after the instructions to record opportunities in `Table \ref{tab:session4-opportunity-template}` (around L84–L110).
  **Draft content:** “Before class, each team member should have at least five opportunities recorded using the template with fields for description, charter alignment, expected value and physics/technical focus. Verify that each entry notes the relevant physics or technical aspect.”
  **Rationale:** Ensures completeness and quality of recorded options.

* [ ] **Common Mistakes** before the Screening Criteria subsection (around L127).
  **Draft content:** “Don’t fixate on one idea too early. The goal here is to explore the design space broadly. Avoid ideas that fall outside your charter or lack technical depth. Be honest about feasibility—if the team cannot develop or study it within the course, remove it from consideration.”
  **Rationale:** Encourages objective screening.

* [ ] **Checkpoint** after the Screening Matrix instructions (around L152).
  **Draft content:** “Complete the screening matrix using a 1–5 scale for alignment, impact, feasibility, technical depth and resource fit. Retain only those opportunities that score well on most criteria, and record the rationale for discarding others.”
  **Rationale:** Reinforces disciplined selection and documentation.

---

## Sessions 5 & 6 – Product Planning

**Summary:** Sessions 5 and 6 transform the shortlisted opportunity into a clear mission statement by performing market analysis, identifying relevant technologies, stakeholders and constraints, and drafting then refining a mission statement. Session 5 is individual preparation; Session 6 is group consolidation. The chapter stresses the importance of market segments, technology integration, manufacturing and service objectives, target market and price, assumptions and constraints, and stakeholder analysis. Templates are provided for both individual and group analyses.

### Proposed insertions

### Session 5 (individual analysis)

* [ ] **Goal** near the start of Session 5 (immediately after the description of the two-session overview).
  **Draft content:** “In Session 5, each team member will conduct a market analysis for the selected hydroponic product and draft a mission statement. Identify relevant market segments, potential technologies, manufacturing and service constraints, realistic price ranges, assumptions and constraints, and key stakeholders. Draft a concise mission statement that summarises your findings.”
  **Rationale:** Frames the individual tasks clearly.

* [ ] **Hint** adjacent to Activity 1 (market analysis).
  **Draft content:** “Don’t limit your thinking to user demographics. Consider physical behaviours—flow stability, corrosion resistance, thermal exposure, sensor accuracy—and how these influence technology choices. Use credible sources (market reports, academic articles, industry publications) to support your analysis, and note any assumptions or uncertainties.”
  **Rationale:** Encourages deeper, physics-aware research.

* [ ] **Checkpoint** after the market analysis template (`Table \ref{tab:session56-market-analysis}`).
  **Draft content:** “Complete all rows in the market analysis table—market segment, technology opportunities, manufacturing/service issues, target market and price, assumptions and constraints, and stakeholders. Include sources or notes for each entry. Without a thorough analysis your mission statement will lack foundation.”
  **Rationale:** Ensures completeness.

* [ ] **Hint** before Activity 2 (mission statement drafting).
  **Draft content:** “A good mission statement includes: a concise product description, the benefit proposition, key business goals, primary and secondary markets, assumptions and constraints, and stakeholders. Use the drafting template and write in clear, actionable language.”
  **Rationale:** Guides students to include all required elements.

* [ ] **Checkpoint** after the mission statement template (`Table \ref{tab:session56-mission-template}`).
  **Draft content:** “Draft your mission statement and verify that it contains all seven fields—product description, benefit proposition, primary market, secondary market, key goal, assumptions/constraints, and stakeholders. Keep it short and precise; avoid technical solutions at this stage.”
  **Rationale:** Encourages thoroughness and alignment with the opportunity.

### Session 6 (group consolidation)

* [ ] **Goal** at the start of Session 6.
  **Draft content:** “In Session 6, your team will merge individual analyses into one shared plan and mission statement. Agree on market segments, technology opportunities, manufacturing/service considerations, target market and price, assumptions and constraints, and stakeholders. Finalise a mission statement that reflects consensus and evidence.”
  **Rationale:** Emphasises synthesis and agreement.

* [ ] **Checkpoint** after the Group Consolidation Template (`Table \ref{tab:session56-group-consolidation}`).
  **Draft content:** “Record the final consensus for each planning element and cite the evidence or rationale. Ensure that all voices are heard and that unresolved disagreements are noted. This consolidated table will guide Sessions 7 and 8.”
  **Rationale:** Ensures documentation of group decisions.

* [ ] **Common Mistakes** near the final mission statement activity.
  **Draft content:** “Avoid mission statements that are too vague (‘make hydroponics easier’) or too ambitious for the course. Check that your mission is consistent with the innovation charter and shortlisted opportunity, includes realistic assumptions and constraints, and provides enough technical direction for customer-needs analysis.”
  **Rationale:** Guards against misalignment.

* [ ] **Hint** at the end.
  **Draft content:** “Use your final mission statement as a touchstone in later sessions. When specifying needs, metrics, functions, concepts, and tests, continuously ask whether the choices support this mission.”
  **Rationale:** Promotes continuity across chapters.

---

## Session 7 – Customer Needs

**Summary:** Emphasises generating survey prompts, translating customer statements into needs, considering lead and extreme users, and building a structured needs table. Key definitions of customer statement, needs statement, lead user and extreme user are provided. The chapter underscores the role of customer needs in connecting the mission statement to measurable specifications.

### Proposed insertions

* [ ] **Goal** after the learning objectives (after L19).
  **Draft content:** “The objectives today are to prepare survey or interview prompts, translate customer statements into concise needs statements, consider whether lead or extreme users should be consulted, and build a structured needs table for your product.”
  **Rationale:** Provides a quick checklist of tasks.

* [ ] **Hint** near the survey design guidelines (around L68–L88).
  **Draft content:** “Frame questions around typical use, likes, dislikes and suggested improvements. Ensure questions are clear, concise and unbiased. Whenever possible, justify why each question is useful to your project.”
  **Rationale:** Reinforces good survey practice.

* [ ] **Checkpoint** below `Table \ref{tab:session7-question-template}` (around L98–L122).
  **Draft content:** “Before class, each member should produce at least three survey questions with corresponding justifications. Make sure your prompts cover monitoring habits, pain points and improvement suggestions, as shown in the example table.”
  **Rationale:** Ensures preparation.

* [ ] **Common Mistakes** near the translation guidance section (around L146–L155).
  **Draft content:** “Don’t rewrite customer statements as solutions (e.g., ‘use a float sensor’). Needs statements should describe what the product must enable or improve. Avoid assumptions or biases; keep statements concise and specific.”
  **Rationale:** Helps distinguish needs from solutions.

* [ ] **Hint** in the lead/extreme user activity.
  **Draft content:** “Reflect on whether interviewing lead users (experienced growers who face problems early) or extreme users (those in challenging conditions) will reveal hidden needs. Consider their potential to expose edge cases that typical users might miss.”
  **Rationale:** Encourages critical thinking about user selection.

* [ ] **Checkpoint** after the description of the needs table (where Table `tab_hydroponic_user_needs` is introduced).
  **Draft content:** “Your group table must include agreed survey prompts, customer statements organised by themes, the interpreted needs statements and the variable type. Optionally, indicate whether each need is direct, latent, constant, variable, general or niche. This table is the foundation for specifications in Session 8.”
  **Rationale:** Emphasises completeness and future use.

---

## Session 8 – Product Specifications

**Summary:** Transforms interpreted needs into measurable specifications. Tasks include assigning importance scores to needs, defining metrics and units, evaluating metrics against guidelines, and compiling benchmark information. The chapter cautions against over-reliance on unverified LLM outputs and provides guidelines for choosing metrics.

### Proposed insertions

* [ ] **Goal** after the objectives list (around L17).
  **Draft content:** “Today you will convert needs into measurable specifications. Assign relative importance to each need, define candidate metrics and units, evaluate those metrics using guidelines (reflect customer needs, allow design freedom, be practical to measure, accommodate subjective needs and enable market comparison), and collect benchmarking data.”
  **Rationale:** Summarises tasks and guidelines.

* [ ] **Checkpoint** after the importance table description (around L38–L50).
  **Draft content:** “Complete a needs-importance table by assigning a 1–5 importance score to each need based on frequency, impact and alignment with your mission. Record the reason for each score.”
  **Rationale:** Verifies that importance ranking is done before moving to metrics.

* [ ] **Common Mistakes** after the discussion on using LLMs (around L81–L122).
  **Draft content:** “LLM suggestions are drafts only. Verify each proposed metric using engineering judgement, credible sources and the logic of your project. Avoid metrics that over-constrain the design or fail to reflect the underlying need.”
  **Rationale:** Encourages critical assessment of AI-generated content.

* [ ] **Hint** in the Metric Selection Guidelines section (around L108–L123).
  **Draft content:** “For each candidate metric, indicate which guidelines it satisfies:

  1. reflects customer needs,
  2. allows design freedom,
  3. is practical to measure,
  4. applies to subjective needs, or
  5. supports market comparison.
     When possible, choose metrics that cover multiple categories.”
     **Rationale:** Guides students to use the guidelines explicitly.

* [ ] **Checkpoint** at the end of the metric table description (around L125–L127).
  **Draft content:** “Ensure your metric table lists each need, the proposed metrics, units, justification and the guideline numbers satisfied. Without these columns you cannot build a robust need-metric matrix.”
  **Rationale:** Enforces completeness.

* [ ] **Checkpoint** after the benchmarking activity description (referencing the comparison table).
  **Draft content:** “Collect at least one data point from a competitor or reference product for each of your key metrics. Record the source and be prepared to justify why the reference is relevant. If no competitor data exists, explain how you estimated an initial target.”
  **Rationale:** Ensures realistic benchmarks.

---

## Session 9 – Functional Decomposition and Solutions

**Summary:** Introduces functional decomposition, encourages teams to choose an approach (functional, sequence of user actions, or key customer needs), decompose the product into verb–noun pairs, produce a requirement–function matrix, and search for multiple solutions to critical sub-functions.

### Proposed insertions

* [ ] **Goal** after the objectives list (around L9–L16).
  **Draft content:** “Your tasks today are to choose a decomposition approach, break your product into generic verb–noun functions, build a requirement–function matrix to verify coverage of needs and specifications, and search for at least five solution options for each critical sub-function.”
  **Rationale:** Clarifies the multi-stage nature of the session.

* [ ] **Common Mistakes** near the definition of functional decomposition (around L20–L24).
  **Draft content:** “Don’t jump straight to technical solutions (e.g., ‘use a 12 V pump’)—describe functions generically (e.g., ‘move solution’). Avoid decomposing only by physical components; think in terms of what the product must do.”
  **Rationale:** Prevents premature solution bias.

* [ ] **Hint** in the Decomposition Approaches section (around L28–L39).
  **Draft content:** “Choose the decomposition approach that best suits your product: use functional decomposition for products with interacting subsystems; sequence of user actions for user-centred tasks; or key customer needs if the product is driven by distinct needs. Justify your choice briefly.”
  **Rationale:** Encourages deliberate method selection.

* [ ] **Checkpoint** after the Procedure list (around L50–L57).
  **Draft content:** “Complete a draft decomposition including the overall function, chosen approach and at least three major sub-functions, recorded in the template. Prepare to explain why you selected this approach.”
  **Rationale:** Ensures that each student comes to class prepared.

* [ ] **Hint** in the Solution Search section (around L100–L115).
  **Draft content:** “When brainstorming solutions for each sub-function, consider feasibility, alignment with needs, technical maturity, resource requirements and source credibility. Use a mix of internal brainstorming and external research (papers, patents, datasheets).”
  **Rationale:** Provides evaluation criteria for solutions.

* [ ] **Checkpoint** after the solution search template.
  **Draft content:** “For each critical sub-function, list at least five solution options with sources and feasibility notes. Prepare to merge these into a team table in class.”
  **Rationale:** Ensures thorough exploration of alternatives.

---

## Session 10 – Concept Generation

**Summary:** Builds on the decomposition and solution search by creating a concept classification tree, a concept combination table, generating at least five rough product concepts, and shortlisting promising concepts. It explains why structured tools matter and provides examples.

### Proposed insertions

* [ ] **Goal** after the learning objectives (around L15–L16).
  **Draft content:** “Today you will organise your solution options into a classification tree and a combination table, then generate and describe at least five rough product concepts by combining sub-solutions. Finally, prepare to shortlist concepts for Session 11.”
  **Rationale:** Summarises tasks.

* [ ] **Hint** in the explanation of classification trees and combination tables (around L43–L73).
  **Draft content:** “Group solutions by category (e.g., for a hydroponic product: how to move the solution, how to monitor level, how to support the structure). Use the classification tree to ensure you consider all options before combining them. The combination table is a menu, not a set of final concepts—feel free to mix and match creatively.”
  **Rationale:** Reinforces proper use of tools.

* [ ] **Checkpoint** after the description of rough concepts (around L104–L116).
  **Draft content:** “Generate at least five rough concepts. For each, record a concept name, selected sub-solutions, a short description of how it works, and at least one strength and weakness. These descriptions need not be detailed but must be clear enough for comparison.”
  **Rationale:** Ensures adequate exploration of the design space.

* [ ] **Common Mistakes** before the in-class consolidation section (around L137).
  **Draft content:** “Don’t prematurely pick a favourite concept or combine incompatible sub-solutions. Evaluate whether combinations make sense in terms of physics, maintenance, cost and user needs. Keep multiple options alive until you have evidence to narrow them down.”
  **Rationale:** Encourages open-mindedness and critical evaluation.

* [ ] **Checkpoint** at the end of the shortlist criteria list (around L146–L155).
  **Draft content:** “When selecting concepts to carry forward, consider feasibility, alignment with customer needs and specifications, degree of innovation, integration of relevant physics principles, and potential for development within the course. Document why each shortlisted concept was chosen or discarded.”
  **Rationale:** Promotes transparent justification.

---

## Session 11 – Concept Selection

**Summary:** Narrows rough concepts using structured comparison tools. Students derive selection criteria from needs, specifications and enterprise concerns, build a concept-screening matrix using `+` / `0` / `–` symbols, and decide whether more detailed concept scoring is needed.

### Proposed insertions

* [ ] **Goal** after the objectives list (around L15).
  **Draft content:** “This session will help you select the best concept(s) for development. Define selection criteria based on needs, specifications and enterprise factors, build a concept-screening matrix using a datum concept, interpret the results, and decide whether to perform detailed concept scoring.”
  **Rationale:** Summarises tasks and emphasises evidence-based selection.

* [ ] **Hint** near the section on generating selection criteria (around L30–L50).
  **Draft content:** “Derive criteria from customer needs (e.g., easy monitoring, low maintenance), product specifications (e.g., low leakage, stable flow) and enterprise concerns (e.g., cost, manufacturability, installation ease). Don’t forget physics-related suitability like sensor accuracy or structural stability.”
  **Rationale:** Guides criteria selection.

* [ ] **Checkpoint** after the screening matrix example (around L65–L90).
  **Draft content:** “Complete the concept-screening matrix by choosing a datum concept and rating each alternative with `+`, `0` or `–` for each criterion. Count the number of pluses and minuses for each concept. This will reveal the strongest options.”
  **Rationale:** Ensures the matrix is actually completed.

* [ ] **Common Mistakes** before the discussion on concept scoring (around L105–L116).
  **Draft content:** “Don’t base your final decision solely on intuition or excitement. Use the screening matrix to see where each concept excels or falls short, and avoid discarding a concept just because it scores lower on cost if it excels on critical user needs. If the results are close, consider a weighted scoring matrix.”
  **Rationale:** Encourages objective assessment and warns against bias.

* [ ] **Checkpoint** at the end (around L146–L149).
  **Draft content:** “Ensure you produce a documented shortlist of concepts, along with a clear rationale for why concept scoring was or was not performed. This justification will be needed when you plan concept testing in Session 12.”
  **Rationale:** Promotes thorough documentation.

---

## Session 12 – Concept Testing

**Summary:** Describes how to plan and conduct concept testing. Students define the purpose of the test, choose a survey population and sample size approach, select a survey format, draft evaluation questions, decide how to communicate the concept, consolidate plans in class, and consider ethics and documentation.

### Proposed insertions

* [ ] **Goal** after the objectives list (around L18).
  **Draft content:** “Your final preparatory task is to design a concept test. Decide what you need to learn from potential users, choose an appropriate survey population and sample size, select a survey format (interview, email, online form, etc.), draft evaluation questions, and determine how best to communicate your concept.”
  **Rationale:** Summarises the planning steps.

* [ ] **Hint** next to the survey population guidance (around L52–L64).
  **Draft content:** “Select respondents who resemble your target market, have enough experience to evaluate the concept, and match the product’s price level and maintenance expectations. Even a small sample can yield valuable insights if the selection is thoughtful.”
  **Rationale:** Encourages targeted sampling.

* [ ] **Checkpoint** after the concept-test planning template (around L92–L117).
  **Draft content:** “Complete the planning template with the purpose, target market segment, survey population, sample size approach, survey format, main evaluation questions and communication method. Verify that each field is filled before finalising your plan.”
  **Rationale:** Ensures a comprehensive plan.

* [ ] **Common Mistakes** before the communication method comparison table (around L131–L166).
  **Draft content:** “Don’t choose a high-fidelity communication method (e.g., prototype) if a low-effort method (e.g., sketch or storyboard) suffices. Match the method to the complexity of your concept and the time available. Similarly, avoid surveying people outside your target market just because they are readily available.”
  **Rationale:** Encourages efficiency and relevance.

* [ ] **Hint** in the ethics and documentation section.
  **Draft content:** “When collecting feedback, explain the survey’s purpose, respect respondents’ time, and avoid collecting unnecessary personal information. Keep a record of your final plan, the questions used, and the rationale for your choices.”
  **Rationale:** Reminds students of ethical considerations.

* [ ] **Checkpoint** at the end of the session.
  **Draft content:** “Ensure your team agrees on the final concept-test plan and that all details (purpose, population, format, questions, communication method) are documented for the concept-refinement stage. Use the results to inform the final project narrative.”
  **Rationale:** Ensures closure and sets up the final phase.

# Cross-Chapter Continuity Notes

* **Opportunity → Strategy:** The product and company choices from Session 1 underpin the process decisions in Session 2. A **Checkpoint** in Session 1 requires teams to document those choices, ensuring they have material to justify their development strategy and organisational structure later.

* **Charter → Opportunities → Mission:** The innovation charter from Session 3 sets the boundaries for generating opportunities in Session 4, while the shortlisted opportunities guide the market analysis and mission statement in Sessions 5 & 6. A **Hint** in Session 4 directs students back to their charter during brainstorming. Similarly, a **Common Mistakes** box in Session 6 reminds teams to keep the mission aligned with the charter and selected opportunity.

* **Mission → Needs → Specifications:** The mission statement shapes customer-needs identification in Session 7 and the metrics defined in Session 8. **Hint** boxes encourage students to use the mission as a reference when drafting surveys and translating needs, ensuring consistency. Later, a **Goal** in Session 8 asks students to prioritise needs and choose metrics that reflect these needs.

* **Specifications → Functions → Concepts:** Needs and metrics feed into functional decomposition (Session 9), concept generation (Session 10) and concept selection (Session 11). **Hint** boxes stress the importance of using verb–noun pairs and technology-agnostic functions, and **Checkpoints** ensure enough solution options are generated for later combination. During concept selection, a **Hint** encourages deriving criteria from needs and specifications.

* **Concept → Testing:** The selected concept(s) from Session 11 become the subject of concept testing in Session 12. The **Checkpoint** at the end of Session 11 ensures documentation of the rationale, which supports the design of a focused concept-test plan. **Hint** boxes in Session 12 help align the test population and communication method with the earlier mission and target market.

* **Physics and Technical Depth:** Throughout the handbook, emphasise applied physics relevance: when selecting products (Session 1), drafting charters (Session 3), generating opportunities (Session 4), analysing markets (Sessions 5 & 6), defining needs and metrics (Sessions 7 & 8), decomposing functions (Session 9), and evaluating concepts (Sessions 10 & 11). Several **Hints** remind students to consider flow, sensing, structural loading, energy management and other physics aspects.

# Implementation Guidance for the Editing Specialist

* **Preserve LaTeX structure:** Insert each `tcolorbox` immediately after the specified anchor paragraph or section heading. Avoid placing boxes inside `\begin{table}`, `\begin{tabular}`, `\begin{enumerate}`, or other float environments; instead, insert them between paragraphs or after `\end{enumerate}` blocks to prevent compilation errors.

* **Consistent box style:** Use the same `tcolorbox` options throughout the handbook (only `[title=...]` is specified by this plan). The editing specialist may define global styles in the preamble if desired.

* **Use meaningful anchors:** When adding boxes, preserve section and subsection labels. If the recommended insertion point falls inside a complex environment (e.g., within a list), consider moving the box slightly before or after to maintain proper nesting.

* **Avoid duplicates:** If a session already contains a similar pedagogical element (e.g., a summary paragraph or caution), merge the proposed box with existing text rather than repeating information.

* **Check cross-references:** Some boxes refer to earlier or later sessions. Ensure that cross-references (e.g., `Session \ref{sec:innovation-charter}`) compile correctly and adjust labels if the LaTeX file names change.

* **Prioritisation:** If time is limited, prioritise inserting **Goal** and **Checkpoint** boxes first, as these provide the clearest scaffolding. **Common Mistakes** and **Hint** boxes can be added later.

* **Test compile:** After inserting boxes, compile the LaTeX document to verify that the new environments do not break page layout. Adjust the placement if boxes cause awkward page breaks or overflow.

# Master Checklist

Use the checklist below to track progress during implementation. Each box corresponds to an insertion or a planning phase.

* [ ] Session 1: All proposed boxes inserted and cross-checked.
* [ ] Session 2: All proposed boxes inserted.
* [ ] Session 3: All proposed boxes inserted.
* [ ] Session 4: All proposed boxes inserted.
* [ ] Session 5: Individual analysis boxes inserted.
* [ ] Session 6: Group consolidation boxes inserted.
* [ ] Session 7: Boxes inserted and needs table updated.
* [ ] Session 8: Boxes inserted; metric table expanded with guideline column.
* [ ] Session 9: Boxes inserted; functional decomposition and solution tables prepared.
* [ ] Session 10: Boxes inserted; classification tree, combination table and concept descriptions updated.
* [ ] Session 11: Boxes inserted; screening/scoring matrices completed.
* [ ] Session 12: Boxes inserted; concept-test plan finalised.
* [ ] Cross-chapter continuity: Reviewed and cross-references verified.
* [ ] Repeated misconceptions: Common pitfalls normalised across chapters.
* [ ] Final plan ready: Plan reviewed and ready for editing specialist.
