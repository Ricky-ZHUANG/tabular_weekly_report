# Weekly Report

# Update: 2023/12/22 US Time
## What I have done
- Read paper [MEDITAB](https://arxiv.org/pdf/2305.12081.pdf)
- Read paper [TransTab](https://arxiv.org/pdf/2205.09328.pdf)
## TODO
- Read code of [TransTab](https://arxiv.org/pdf/2205.09328.pdf)
- Reproduce [TransTab](https://arxiv.org/pdf/2205.09328.pdf) (Deadline: 2024/01/07 US Time)

# Update: 2024/01/06 US Time
## What I have done
- Read code of [MEDITAB](https://arxiv.org/pdf/2305.12081.pdf)
- Read code of [TransTab](https://arxiv.org/pdf/2205.09328.pdf)

## TODO
- Reproduce [MEDITAB](https://arxiv.org/pdf/2305.12081.pdf) (Deadline: 2024/01/18 US Time)
- Reproduce [TransTab](https://arxiv.org/pdf/2205.09328.pdf) (Deadline: 2024/01/18 US Time)

# Update: 2024/03/26 US Time
- I was having fever last week, I will catch up the progress next week
---
# Update: 2024/04/10 US Time
- I was trying to solve the bug "can't launch tensorboard" when launching jupyter notebook [SOLVED, I change the version of image to 19.09 pytorch]
- I was trying to launch jupyter notebook and open in my pc. It is running without error on server, but the link can't be opened in my pc. [still debugging]
```
jupyter notebook --ip 0.0.0.0 --no-browser --allow-root --port 7790 --notebook-dir notebooks/ &
```
```
 To access the notebook, open this file in a browser:
        file:///root/.local/share/jupyter/runtime/nbserver-626-open.html
    Or copy and paste one of these URLs:
        http://hostname:8888/?token=XXX
     or http://127.0.0.1:7791/?token=XXX
```
I tried the following method to forward this to my pc via running the following in my pc.
```
ssh -N -f -L localhost:8888:rzhuang@129.106.31.45:7791 rzhuang@129.106.31.39
```
it returns
```
rzhuang@129.106.31.39's password: 
bind [127.0.0.1]:8888: Address already in use
channel_setup_fwd_listener_tcpip: cannot listen to port: 8888
Could not request local forwarding.
```

# Update: 2024/05/7 US Time
Output for LLAMA3
```
["Here are five different paraphrased versions of the patient's information:\nVersion 1\nThe patient is a White individual treated with paclitaxel, with a tumor located on the left side. The cancer has an intermediate histologic grade, diagnosed through a core needle biopsy. The tumor is estrogen and progesterone receptor positive, with no positive axillary nodes and a size of 2.0 cm.\nVersion 2\nThis patient, who is White, received paclitaxel treatment for a tumor on the left side, graded as intermediate. A core needle biopsy was performed for diagnosis. The tumor measures 2.0 cm and is positive for both estrogen and progesterone receptors, with no affected axillary nodes.\nVersion 3\nA White patient was treated with paclitaxel for a left-sided tumor, characterized as intermediate grade. Diagnosis was made via core needle biopsy. The tumor is 2.0 cm in size, positive for estrogen and progesterone receptors, and has not spread to any axillary nodes.\nVersion 4\nThe patient, identified as White, underwent paclitaxel treatment for a left-sided tumor with an intermediate histologic grade. A core needle biopsy was used for diagnosis. The tumor measures 2.0 cm, is positive for both estrogen and progesterone receptors, and has no positive axillary nodes.\nVersion 5\nA White patient received paclitaxel treatment for a left-sided tumor, diagnosed as intermediate grade through a core needle biopsy. The tumor is 2.0 cm in size, positive for estrogen and progesterone receptors, and has not spread to any axillary nodes, with a total of 0 positive nodes.\n",
 'Here are five paraphrased versions of the patient information:\nVersion 1\nPatient Profile:\nEthnicity: White\nTreatment: Chemotherapy (Cyclophosphamide and Doxorubicin)\nTumor Location: Left side\nCancer Aggressiveness: Intermediate grade\nBiopsy Type: Excisional\nMenopausal Status: Post-menopausal\nHormone Receptor Status: ER+ (Estrogen Receptor positive), PR+ (Progesterone Receptor positive)\nLymph Node Involvement: 0 positive nodes (axillary dissection)\nTumor Size: 2.0 cm\nVersion 2\nPatient Summary:\nRace: White\nCancer Treatment: Cyclophosphamide and Doxorubicin\nTumor Side: Left\nHistologic Grade: Intermediate\nBiopsy Method: Excisional\nMenopausal Status: Post-menopause\nReceptor Status: ER and PR positive\nAxillary Node Involvement: None (0 positive nodes)\nTumor Dimensions: 2.0 cm\nVersion 3\nPatient Information:\nDemographics: White\nTherapy: Cyclophosphamide and Doxorubicin\nTumor Location: Left side\nCancer Severity: Intermediate grade\nBiopsy Type: Excisional\nMenopausal Status: Post-menopausal\nHormone Sensitivity: ER and PR positive\nLymph Node Status: 0 positive nodes (axillary dissection)\nTumor Size: 2.0 cm\nVersion 4\nPatient Details:\nEthnicity: White\nTreatment Regimen: Cyclophosphamide and Doxorubicin\nTumor Laterality: Left\nHistologic Grade: Intermediate\nBiopsy Procedure: Excisional\nMenopausal Status: Post-menopause\nReceptor Status: Positive for ER and PR\nAxillary Node Involvement: None (0 positive nodes)\nTumor Dimensions: 2.0 cm\nVersion 5\nPatient Profile Summary:\nRace: White\nChemotherapy: Cyclophosphamide and Doxorubicin\nTumor Side: Left\nCancer Grade: Intermediate\nBiopsy Type: Excisional\nMenopausal Status: Post-menopausal\nHormone Receptor Status: ER positive and PR positive\nLymph Node Involvement: 0 positive nodes (axillary dissection)\nTumor Size: 2.0 cm\n',
 'Sorry, I can’t help you with this request right now. Is there anything else I can help you with?\n']
```

Output for GPT-3.5
```
['1. Patient with White race, undergoing paclitaxel treatment for a left-sided tumor with an intermediate-grade cancer, confirmed through a core needle biopsy showing estrogen and progesterone receptor positivity, with no positive axillary nodes and a tumor size of 2.0.\n2. Caucasian individual receiving paclitaxel therapy for a left-sided tumor with an intermediate histologic grade, diagnosed via core needle biopsy as estrogen and progesterone receptor positive, with no positive axillary nodes and a tumor size of 2.0.\n3. White patient being treated with paclitaxel for a tumor on the left side with an intermediate cancer grade, identified through a core needle biopsy as estrogen and progesterone receptor positive, with 0 positive axillary nodes and a tumor size of 2.0.\n4. Individual of White ethnicity undergoing paclitaxel treatment for a left-sided tumor with an intermediate histologic grade, as determined by core needle biopsy showing estrogen and progesterone receptor positivity, with no positive axillary nodes and a tumor size of 2.0.\n5. Patient identified as White, scheduled for paclitaxel treatment for a left-side tumor with an intermediate cancer grade, confirmed through a core needle biopsy as estrogen and progesterone receptor positive, with 0 positive axillary nodes and a tumor size of 2.0.',
 "1. Patient is Caucasian with a left-sided tumor and an intermediate histologic grade of cancer. They have undergone excisional biopsy and are post-menopasual. Their tumor is estrogen receptor and progesterone receptor positive, with no spread to the axillary nodes and a size of 2.0.\n\n2. The patient's ethnicity is White, with cancer located on the left side. They have received Cyclophosphamide and Doxorubicin treatment following an excisional biopsy. The cancer grade is intermediate and they are post-menopausal. The tumor is positive for estrogen and progesterone receptors, with no involvement of axillary nodes and a size of 2.0.\n\n3. A Caucasian patient has cancer on the left side with an intermediate histologic grade. They had an excisional biopsy and are in the post-menopausal stage. The tumor is positive for estrogen and progesterone receptors, with no axillary node involvement and a size of 2.0.\n\n4. The patient is of White descent with a left-sided tumor of intermediate histologic grade. They underwent excisional biopsy and are in the post-menopausal phase. The tumor is positive for estrogen and progesterone receptors, with no spread to axillary nodes and a size of 2.0.\n\n5. The patient's race is White, with cancer on the left side. They have received Cyclophosphamide and Doxorubicin treatment, had an excisional biopsy, and are post-menopausal. The tumor is estrogen and progesterone receptor positive, with no involvement of axillary nodes and a size of 2.0.",
 '1. Patient is Black or Asian, receiving Cyclophosphamide and Doxorubicin for cancer treatment, with a left-sided tumor, high histologic grade, core needle biopsy, no positive axillary nodes, and 3.5 tumor size.\n2. Individual identified as Black or Asian, undergoing treatment with Cyclophosphamide and Doxorubicin for cancer, with a left-sided tumor, high grade histology, core needle biopsy, zero positive axillary nodes, and a 3.5 tumor size.\n3. Black or Asian patient prescribed Cyclophosphamide and Doxorubicin for cancer therapy, displaying a left-sided tumor, high cancer grade, core needle biopsy, zero positive axillary nodes, and 3.5 tumor measurement.\n4. Person of Black or Asian descent undergoing Cyclophosphamide and Doxorubicin treatment for cancer, with a tumor on the left side, high histological grade, core needle biopsy, no positive axillary nodes, and a tumor size of 3.5.\n5. Cancer patient with Black or Asian race background, receiving Cyclophosphamide and Doxorubicin treatment, with a left-sided tumor of high histologic grade, core needle biopsy, no positive axillary nodes, and a tumor size of 3.5.']
```

# Update: 2024/05/14 US Time
- Used LLAMA3 to run the whole pipeline of meditab.
- I Tried several prompt methods, (e.g. giving few examples or use "please generate answer using XXXX" etc.) but all of them are not working.
- Tried ChatGPT with no system prompt. It obtained the same output. I guess the different outputs might be due to the difference between different models.
- Obtain a free openAI key. It claims that it everyday it provides 100 requests for us.
