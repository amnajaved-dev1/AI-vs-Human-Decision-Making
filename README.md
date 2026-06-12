# AI vs Human Decision-Making: A Comparative Analysis

## Overview
This project compares how humans and AI systems make decisions across real-life scenarios involving ethics, emotions, risk, and logic. It uses data analytics, statistical testing, and machine learning to identify behavioral differences between human and AI decision patterns.

## Objectives
- Compare AI and human decision-making patterns across 31 real-life scenarios
- Apply statistical tests (T-Test, Chi-Square, Cohen's d) to measure significance
- Build classification models (Logistic Regression, Random Forest, XGBoost) to distinguish human vs AI responses
- Use Explainable AI (SHAP, feature importance) to interpret model behavior
- Examine ethical, legal, and professional implications of AI decision-making

## Methodology
1. **Data Collection** — Responses gathered via Google Forms from human participants and multiple AI tools (ChatGPT, Gemini, DeepSeek, Claude, etc.)
2. **Preprocessing** — Cleaning, deduplication, encoding, normalization
3. **EDA** — Boxplots, radar charts, scatter matrices comparing response distributions
4. **Statistical Testing** — T-Test, Chi-Square, Cohen's d effect size
5. **Machine Learning** — Logistic Regression, Random Forest, XGBoost classification
6. **Explainability** — SHAP analysis and feature importance ranking

## Tools & Technologies
Python · Pandas · NumPy · Scikit-learn · XGBoost · SHAP · Matplotlib · Seaborn · Google Colab

## Key Findings
- AI and humans often align on logical/factual decisions
- Humans show stronger emotional, ethical, and experience-based reasoning
- AI responses are more consistent and pattern-driven
- Ethically sensitive questions (Q20, Q17, Q16, Q2) had the highest feature importance in distinguishing AI from human responses
- Classification models achieved moderate-to-strong separation, with XGBoost performing best

## Ethical & Legal Considerations
The study also evaluates algorithmic bias, transparency, privacy, and compliance with GDPR and PECA, referencing IEEE, ACM, and BCS ethical codes.

## Conclusion
> AI can imitate certain human decision patterns, particularly in logical scenarios, but human decisions remain more emotional, ethical, and experience-driven, while AI decisions are more consistent and data-driven. AI should support — not replace — human judgment, especially in ethically sensitive contexts.

## Authors
Amna Javed · Ayesha Saleem · Hajra Iftikhar · Hifsa Kanwal
Department of Computer Science, Fatima Jinnah Women University

## Survey Form
[Original data collection form](https://docs.google.com/forms/d/e/1FAIpQLSejs1I8RTYvIyYQ3eJI3UDdUFd78tQr_opf79feFjbwkRbbrg/viewform)
