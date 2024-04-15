# ADViRDS
The dataset for ADViRDS: Assessment of Domestic Violence Risk Dataset and Scale on Social Media in CogSci 2024.

## Introduction
This study presents ADViRDS, an innovative scale and dataset specifically developed for examining the psychological traits of domestic violence (DV) perpetrators. Recognizing the critical need to understand the psychological dynamics of perpetrators, our research shifts the focus from the experiences of DV victims to the characteristics of the perpetrators.

Our approach involves a six-dimensional scale designed to detect the psychological traits of DV perpetrators, formulated with insights from established DV research and psychologists. To complement this scale, we constructed a detailed dataset containing 591 individual entries from the Chinese social media platform "Zhihu." Each entry was carefully annotated by experienced professionals, ensuring a high degree of accuracy and relevance.

We conducted a comprehensive analysis using a range of models, including Zero-Shot classification, GPT series, and fine-tuned pre-trained models, to evaluate their effectiveness in identifying individuals with psychological predispositions to DV. The findings reveal significant insights into the models' capabilities, highlighting the nuances in detecting DV tendencies through psychological profiling.
Our research offers a new paradigm in DV studies, focusing on the psychological traits of perpetrators for a comprehensive understanding of DV dynamics and prevention.

## Scale
We collaborated with seasoned psychologists to construct a DV psychological characteristics scale. The scale is designed with six dimensions to provide a comprehensive analysis of the psychological traits of DV perpetrators. These dimensions collectively encompass various aspects, offering a thorough and multidimensional understanding of their characteristics.

| Category                  | Description                                                                                               | Example                                                                                                                                                      |
|---------------------------|-----------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------|
| *Trauma Experience*       | Poverty, physical abuse, sexual abuse, cold violence, emotional abuse, emotional neglect, etc.             | *"I heard my grandfather beat my grandmother even worse. My dad also resents this; he used to tell us about how he was beaten as a child, how his mother was beaten..."* |
| *Misconduct*              | Gambling, alcohol abuse, drug misuse, drug addiction, overspending, etc.                                  | *"When I was young, my dad loved gambling and he would ask my mom for more money. If she didn't give him money, he would instantly rage, drag her into the bedroom, lock the door, and beat her brutally..."* |
| *Personality Deviation*   | Obvious jealousy, suspicion, paranoia, cold-heartedness, etc.                                             | *"Now he still has a very strong desire to control, even to the extent of being paranoid about whom my sister dates..."*                                     |
| *Emotional Dysregulation* | Impulsiveness, easy to anger, irritability, strong desire for control, poor self-control, etc.            | *"He, like a madman, pressed me into a corner and hit my head with a hot water kettle. He is irritable and unable to control his emotions, often getting into conflicts with others..."* |
| *Cognitive Bias*          | Significant deviation from mainstream understanding: black-and-white thinking, overgeneralization, absolutism, labeling, personalization, mind reading, shoulds and musts, emotional reasoning, etc. | *"After I started a relationship with my boyfriend, he always implied that he was superior and I was inferior. He belittled me to elevate himself, obstructed my normal social life, forbade me from seeing friends..."* |
| *Violent Tendencies*      | History of violence, animal abuse, hitting people in childhood, threatening others, damaging property, etc. | *"Last night, because two cats at home fought, my boyfriend beat one of them severely. He even said he wanted to kill it. When I calmly told him to do it, he immediately went down to continue the beating..."* |


## Dataset

### Format
`ADViRDS_data.json`: Contains 574 posts with each post having the following attributes:
* `id`: id of the post
* `entity`: individual with domestic violence tendency in the post
* `content`：the entire text of the post
* `conditions`: determination labels for each dimension in the scale
    1. C1~C6：conditions(dimensions) in the scale
    2. **1/0** label depending on whether "it is possible to use the content in the post text to infer/it is known that the entity has a problem corresponding to the condition"


## Citation
