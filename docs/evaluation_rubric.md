# Evaluation Rubric for Financial LLM Research Tools

Use this rubric for evaluating LLM outputs in financial and macroeconomic research workflows.

## What Is a Rubric?

A rubric is a structured scoring framework. In this project, it converts qualitative judgments such as "the answer looks good" into more transparent criteria, such as factual accuracy, evidence grounding, citation quality, risk awareness, and reproducibility.

In Chinese, this can be understood as `评测量表` or `评分标准`. It helps make evaluation more standardized, especially when comparing RAG systems, agent workflows, or macro research assistants.

## 为什么需要 Rubric？

金融和宏观研究里的大模型输出不能只看语言是否流畅，还要看：

- 事实是否准确；
- 有没有可靠证据支持；
- 引用是否对应原始材料；
- 推理链条是否清楚；
- 是否意识到数据和模型局限；
- 输出是否可以复现和审计。

因此，rubric 的价值在于让评测更像研究流程的一部分，而不是主观印象。

| Dimension | Question | Strong Output |
| --- | --- | --- |
| Factual accuracy | Are financial, institutional, and macroeconomic facts correct? | Uses correct terminology, dates, institutions, and economic relationships. |
| Evidence grounding | Are claims supported by retrieved sources? | Cites relevant evidence and distinguishes evidence from inference. |
| Reasoning quality | Does the output explain assumptions and causal logic? | Shows transparent reasoning without overstating certainty. |
| Domain relevance | Is the answer useful for financial research? | Focuses on market, policy, macro, and institutional implications. |
| Risk awareness | Does it identify limitations and possible failure modes? | Notes data gaps, model limits, uncertainty, and policy sensitivity. |
| Reproducibility | Can another researcher trace the workflow? | Provides source metadata, retrieval logic, and structured outputs. |
| Communication | Is the output concise and professional? | Uses clear research language suitable for memos or reports. |
| Citation precision | Do citations point to the correct source passages? | Links claims to the right document section or source note. |
| Numerical discipline | Are numbers, dates, and units handled correctly? | Avoids invented numbers and preserves source units and time periods. |
| Uncertainty handling | Does the output communicate uncertainty properly? | Uses calibrated language and avoids unsupported certainty. |
| Policy sensitivity | Does the output avoid overclaiming in policy contexts? | Clearly separates evidence, interpretation, and recommendations. |
| Robustness | Does the answer remain stable under prompt variation? | Gives consistent conclusions when the question is rephrased. |
| Data limitation awareness | Does it discuss data coverage and bias? | Notes missing data, publication lags, revision risk, and selection bias. |
| Audit trail quality | Can the process be inspected after generation? | Preserves retrieval logs, source IDs, prompt version, and model settings. |

## Suggested Scoring

Use a 1 to 5 scale for each dimension:

- 1: Poor or unsupported.
- 2: Partially relevant but unreliable.
- 3: Acceptable with limitations.
- 4: Strong and mostly complete.
- 5: Excellent, evidence-grounded, and ready for research use.

## Suggested Evaluation Sheet

| Output ID | Task | Model / Workflow | Score 1-5 | Main weakness | Reviewer note |
| --- | --- | --- | --- | --- | --- |
| OUT-001 | Policy memo draft | RAG baseline |  |  |  |
| OUT-002 | Macro theme extraction | Agent workflow |  |  |  |
| OUT-003 | Literature summary | Retrieval + summarizer |  |  |  |
