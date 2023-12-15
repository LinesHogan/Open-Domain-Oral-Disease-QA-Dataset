# Open-Domain-Oral-Disease-QA-Dataset
Dataset and basic implementation reference of the paper: Evaluate the ability to self-diagnose oral diseases of large language models: an exploratory, proof-of-concept study 

## Dataset Overview

### Available Datasets
We currently offer a suite of evaluation datasets encompassing models such as GPT-3.5, GPT-4, Palm2, and Llama2-70B. More data is under reviewed. This dataset is meticulously designed to evaluate the diagnostic capabilities of Large Language Models (LLMs) in the domain of oral disease. 

### Immediate Access
For immediate access to our review datasets, please reach out to Yuanhao Zeng at cengyuanhao@bupt.edu.cn.

### Dataset Format
Our datasets are structured in the JSON Lines (jsonl) format, where each line encapsulates a comprehensive conversation context. This includes manual evaluation results and meta-information vital for machine learning model training.

### Data Schema
The datasets adhere to the following key-value schema:
```json
{
    "LLM":"LLM type",
    "Disease": "Ground Truth Disease Type",
    "Validity": "Manual Evaluation of LLM Response Validity",
    "Necessity": "Urgency Rating of LLM Response Based on Manual Evaluation",
    "Question": "Medical-Related Query",
    "Answer": "LLM Generated Response"
}
```

### Example

```json
{
    "LLM":"llama-2",
    "disease": "malocclusion",
    "validity": "correct",
    "necessity": "important",
    "question": "My upper and lower teeth don’t align when I close my mouth. Does this mean I am sick? If so, can you give me a diagnosis?",
    "Answer": "It's possible that your teeth not aligning properly when you close your mouth could be a sign of a dental issue, but it's not necessarily a sign of illness. Here are a few potential causes:\nMalocclusion: This is a term used to describe a misalignment of the teeth, where the upper and lower teeth don't fit together properly. Malocclusion can be caused by a variety of factors, including genetics, injury, or uneven tooth wear.\nOverbite or underbite: An overbite occurs when the upper teeth overlap the lower teeth too much, while an underbite occurs when the lower teeth overlap the upper teeth too much. Both of these conditions can cause teeth misalignment.\nCrowded or crooked teeth: If your teeth are crowded or crooked, they may not align properly when you close your mouth.\nGum recession: If your gums have receded, the roots of your teeth may become exposed, which can cause teeth misalignment.\nTooth loss: If you have lost one or more teeth, the surrounding teeth may shift out of place, leading to misalignment.\nIt's important to note that teeth misalignment can cause a variety of oral health issues, such as tooth wear, gum irritation, and difficulty chewing or biting.\nIf you're concerned about your teeth alignment, it's best to consult with a dentist. They can examine your teeth and determine the cause of the misalignment. Depending on the severity of the issue, your dentist may recommend one or more of the following treatments:\nOrthodontic treatment: This can include braces, aligners, or other appliances to help straighten your teeth and improve alignment.\nDental crowns or veneers: These can be used to cover and reshape teeth that are severely misaligned or have been damaged.\nGum grafting: If gum recession is contributing to teeth misalignment, a gum graft may be performed to cover exposed roots and improve gum health.\nDental implants: If you have lost teeth, dental implants can be used to replace them and improve overall alignment.\nIn summary, teeth misalignment can be a sign of an oral health issue, but it's not necessarily a sign of illness. It's important to consult with a dentist to determine the cause of the misalignment and develop an appropriate treatment plan.\n"
}
```

# Basic implementation

Coming soon ...
