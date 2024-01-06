# MediTab
T = \{T1, T2 ... Tn\} T1 means the task to learn
- Consolidation: Convert each table's col into natural language description
- Learn: Take the original T1 and train a model f, then f can be used to predict the y of other tables
- Annotate: Use f (model learned from previous learning) to predict the y of other T\*, get T~ which contains noisy label
- Audit: Calculate shapely value. Then filter out low quality rows by this value, get T_clean
- Learning: pre-train the model by T_clean; finetune using T1

# TransTab
- The input is divided into three categories, category, number and binary, and for each category, there is a corresponding to token method. Each token will be concatenated later.
- The tokens are input to the multiple gated transformers.
- The output is used for supervised learning and contrastive learning.

# Difference
- MediTab used LLM to convert columns into description and convert into token. TransTab convert original column into token.
