# Causal-Inference-in-Multisensory-Perception
Exploring a model that explains how individuals integrate auditory and visual stimuli.

*   **The Problem of Causal Inference in Perception**:
    *   Sensory cues are rarely ecologically relevant on their own; their meaning comes from their causes.
    *   The nervous system constantly combines uncertain information from different sensory modalities to understand the causes of stimulation.
    *   Traditional probabilistic models often assume a single variable in the world causing the cues (e.g., a single animal position causing both auditory and visual information), which are then combined optimally using Bayesian statistics.
    *   However, evidence suggests that this "forced-fusion" idea is not always true; integration breaks down with large disparities between stimuli. When events are far apart in space, time, or structure, subjects tend to infer two independent causes rather than a single one.
    *   Von Helmholtz had suggested that multiple objects could cause sensations, implying that two sensory signals might have a common cause (requiring integration) or different independent causes (requiring separate processing).

*   **The Causal Inference Model**:
    *   This model formalises the problem of causal inference and the choice between integration and segregation in multisensory perception.
    *   It operates as an **optimal Bayesian observer** that not only infers the location(s) from two sensory signals (visual and auditory) but also determines whether these signals share a **common cause (C)**.
    *   The model considers two hypotheses: either a common cause or independent causes.
    *   Cues are **fused** if the model infers one common cause, and **segregated** if it infers independent causes. When there's uncertainty about the causal interpretation, it continuously adjusts cue combination based on the **degree of belief** in the causal structure.
    *   It uses two pieces of information: the **likelihood** (sensed visual and auditory positions, corrupted by noise) and the **prior** (how likely two co-occurring signals are to have a common cause versus two independent causes, based on experience).
    *   The model depends on four parameters: **uncertainty of vision (sV)**, **uncertainty of audition (sA)**, **spatial layout prior (sP)** (representing a bias to perceive stimuli centrally), and the **prior probability of a common cause (pcommon)**. These parameters are fitted to human behaviour.
    *   **Key predictions** of the model include:
        1.  The circumstances under which subjects perceive a common cause or independent causes.
        2.  Whether individual cues should be fused or processed separately.
        3.  How cues are combined when they are integrated.

*   **Experimental Evidence and Model Performance**:
    *   **Experiment 1 (Auditory-visual spatial localization)**:
        *   Used a laboratory version of the ventriloquist illusion, where simultaneous auditory and visual stimuli were presented with varying spatial disparities, and subjects reported both perceived locations.
        *   **Findings**: Vision influenced auditory estimates. The causal inference model **accurately predicted human nonlinear cue integration** and explained the data very well (R2 = 0.97). It fits the data better than other traditional models, including "pure integration" (forced-fusion) or "pure segregation" models (Table 1).
        *   The model also naturally predicted that **bias (influence of vision on audition) decreases with increasing spatial disparity**.
        *   Fitted parameters indicated vision (sV = 2.14u) is more precise than audition (sA = 9.2u), subjects have a modest central bias (sP = 12.3u), and the average probability of perceiving a common cause (pcommon = 0.28u) is relatively low.
    *   **Experiment 2 (Auditory-visual spatial localization with measured perception of causality)**:
        *   Compared the model's predictions with data where subjects explicitly reported their perception of unity (common vs. two causes).
        *   **Findings**: The model explained **human perception of causality** well (72% of variance), showing that closer stimuli lead to a higher perception of a common cause.
        *   Crucially, the model accounted for the **counterintuitive finding of negative biases**. This means when subjects perceived distinct causes, their auditory location estimate was pushed *away* from the visual stimulus, not just relying solely on the auditory input. The model explains this as a **selection bias**; trials where distinct causes are inferred are those where the internal auditory signal representation happens to be far from the visual signal.

*   **Broader Implications**:
    *   The causal inference model provides a **normative framework** for understanding multisensory perception, explaining why models utilizing an "interaction prior" have been successful.
    *   It presents a partial answer to the **perceptual binding problem** – how sights and sounds are paired into a unified conscious percept.
    *   Many previous models of cue combination are considered **special cases** of this causal inference model.
    *   The authors suggest that the brain may have evolved highly effective solutions for problems crucial to everyday life, making ideal observer models good predictors of human behaviour in such contexts.
    *   An **intriguing link** is drawn between causal inference in sensory integration and that in higher-level cognition; the optimal statistical principles are very similar, suggesting **common or similar underlying mechanisms** in the brain for inferring hidden causes across perception and cognition.
