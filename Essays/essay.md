---
student_name: Katriina Parkkinen
topic: How does the open weight model from gpt-oss-safeguard and ROOST align with digital commons and can online safety be community-led?
---

# Introduction

On October 29th 2025, OpenAI and ROOST published the open source weights of gpt-oss-safeguard, a bring-your-own-policy model that allows developers to fine-tune safety classification tasks with the aim of making moderating online spaces easier. The model uses chain-of-thought reasoning, explaining the decision it takes to create transparency for the organizations using it. 

The model is available as a research preview under the Apache 2.0 license, allowing it to be used, modified, and deployed freely, and it can be downloaded from Hugging Face in 20b or 120b versions. 

Alongside the model, a ROOST Model Community (RMC) repository was published on GitHub to build an open source community. These are said to be a part of the online safety commons ecosystem.

## How it works

With the gpt-oss-safeguard developers can draw policy lines that best fit their use case, the model explains how the content is classified under the given policy, and developers can then decide if they want to use the model conclusion in their safety pipelines. It differs from traditional safety classifiers by interpreting the policy at the time it is passed into the model instead of training the model on a large number of labeled examples. This creates a level of flexibility, as the models output is also explained, allowing for a more iterative process where the input can be tweaked for the model to interpret it more accurately. 

OpenAI states that traditional classifiers can have high performance, with low latency and operating costs, but gathering sufficient training examples can be costly and time-consuming, and the classifier needs to be re-trained if the policy is updated or changed. From a product perspective, a model that can intake any policy to apply reasoning to is not only more efficient, but also safer as content online is ever-evolving and there may be a lag between the classifiers and new content. However, this can also increase the compute costs and latency. OpenAI has also stated that the traditional dedicated classifiers still perform better which may be preferred for complex risks, so there remains trade-offs.

# Online safety and digital commons

ROOST has stated that they develop AI and safety tools with an open source model to benefit from interoperability, support informed governance, and make technology development more efficient. The partnership with OpenAI is said to improve real-world safety as the risk is not as oncentrated as it is in closed systems. Similarly to digital commons, small-scale developers can access resources they may not usually have access to and they do not need to rely on off-the-shelf solutions that are not suited for specific needs.

## Elinor Ostrom’s 8 principles for governing the commons

The gpt-oss-safeguard is assessed using the eight principles for governing the commons. This is aimed at looking what about this model works and what may need improvements with the goal of fairly assessing the model as a potential commons when creating policy. 

### 1. Clearly defined boundaries

The weights of the model are publicly available under the Apache 2.0 license, similarly to the previously published gpt-oss models. However, it does not fully qualify as a digital commons since the full training data, source code for the training process, and the specific methodology in developing the model are not publicly accessible. It is therefore more open-weight rather than open-source, wording which is also debated in communities such as Reddit asking why it's marketed as open-source when it does not fully qualify the definition. This further separates the model from being a digital commons.

The access to the resource is therefore also separated. Anyone can access the weights, but the ultimate governing community appears to be OpenAI. It's also unclear to what extent the community is able to influence the project as it is still new and unestablished. 

Alignment with first principle: **partial**.

### 2. Rules fit local needs

This principle is strongly aligned as bring-your-own-policy acts as the basis for adapting the safeguards to the local and cultural norms of the project. From the publications from both OpenAi and ROOST, this customization has been the key design principle for the project.

Alignment with second principle: **strong**.


### 3. User participation and decision-making

The ability to change and influence the rules by which the model is developed appears to have been outsourced to ROOST. In their product release post, OpenAI states that ROOST is launching the model community, RMC, whereas OpenAI is only publishing a short technical report to detail the safety perfomance of the preview model.

It seems that there is collective influence informally, such as the stated cooperation at identifying developer needs, testing the model and producing developer documentation when the model was first developed, and now the continuing community engagement driven by ROOST. However, there appears to be a lack of formalized mechanisms for contibutors to influence upstream design decisions or the roadmap priorities at OpenAI.  It therefore remains unclear how much community members are able to participate in the decision making process.


Alignment with third principle: **partial**.

### 4. Monitoring

There are two identified levels for monitoring of the models: one by the community RMC (and other developers contributing on GitHub) and one by OpenAI.

The community monitoring works similarly to the commons in general, with code released in a GitHub repository abd Hugging Face, allowing collaborative issue tracking, bug resolution and overall sharing of knowledge more freely. Researchers and developers can also make their own analyses and comparisons to establish performance and limitations according to their benchmarks. There are also additional communities, such as the OpenAI developer community, that can be used for cooperation and collaboration. Overall, these open communities foster accountability and effective monitoring.

OpenAI's approach to monitoring of the model is unclear, as established in principle 3, but it can be assumed that they have their own evaluation protocols they enforce. Since the source code is not published, there are likely monitoring capabilities built-in or an internal accountability framework. This is also echoed when OpenAI stated that the safeguard model is an open-weight implementation of an internal approach, meaning that before the weights are a result of iterative, closed development which may have stricter monitoring. It is also important to raise that the model itself is designed to be accountable by providing reasoning for its decisions, so it can be argued that monitoring is inherent in the model.

Alignment with fourth principle: **strong**.

### 5. Graduated sanctions

This principle is difficult to assess as the model is new and the use cases are limited. There is no specific mention of sanctions on either ROOST or OpenAI sites or other mentions actions to be taken. This could also be due the model being published as a research preview first, making its expected user base a homogeneous group that may not require the same type of sanctioning. 

OpenAI has entity-level usage policies it says applies to all its products, however how these are enforced in the gpt-oss environment remains unclear. There has been criticism in the developer community that the models are "obsessed" with the content policy where its impacting the model performance. A game developer in a Hugging Face community post said that the model they used (openai/gpt-oss-20b) started to be suspicious of the input and whether is complied with the content policy to the point where is forgot some of the context it was meant to consider. 

Overall the sanctioning principle remains unclear, but there seems to be a strong correlation with the overall OpenAI use policy. It is unclear if the responses are proportonal to the violations.

Alignment with fifth principle: **weak/unclear**.

### 6. Conflict resolution

Building upon the previous principles, the unclear community structure also makes assising the sixth principle difficult. Based on the product releases, there is no built-in dispute resolution process. ROOST supports an informal community forum but this can be an informal resolution channel so its effectiveness is unclear. 

Alignment with sixth principle: **weak/unclear**.

### 7. Right to organize

This principle can be layered depending on how its looked at (as AI or as code or as a safety tool) and who uses it. In the EU, this could be an alternative or a tool for "trusted flaggers", special entities under the DSA, who are responsible for flagging illegal content to online platform providers. This provides a potentially large benefit as it could make the governance of online safety more robust. 

However, there are still open questions about how this fits under the EU AI act (e.g. potential classificiation as a high risk system and this effects development), if the explanation provided is transparent enough, and if it can be supported as a commons.

Alignment with seventh principle: **moderate**

### 8. Embedded in larger networks

Integrating oss-safeguard into layered governance structures is still emerging and therefore needs time to be realised. However for ROOST this is more clear with them being the larger ecosystem that is governing online safety. They can also then better function in larger networks themselves. It remains to be seen how well the safeguard model can embedded, but from a smaller organisation perspecive it does appear more likely.

Alignment with eighth principle: **moderate**

# Conclusion

Governing online safety as a commons or framing online safety as a digital commons allows it to become a shared resource, benefit from shared governance and has the potential for combating rising harms faster and more efficiently. The gpt-oss-safeguard model is a way to make online safety a more accessible issue which hopefully raises it as a priority and an issue people want to work on. However, these are still structural tensions from when this tool is intoduced by a big tech company, and how it can be governed as a commons. 

The open weight model is aimed at smaller entities where developers are able to input their own policy and see how well content can be moderated based on it. The model is however less robust than bespoke classifiers which makes it a less suitable choice for larger entities. It also does not fit the criteria of being a digital commons. It is strongly aligned with fitting local needs and monitoring, but falls short on the remaining principles.

The unclear governance structure remains an issue with the model. To become an efficient digital commons, the boundaries need to be strenghthen along with the decision-making structure. This can make the community more willing to develop the commons as there is clarity, members feel like their contribution matters, and the whole project is not only seen as being controlled by big tech.

# References
Hugging Face: https://huggingface.co/collections/openai/gpt-oss-safeguard  
OpenAI Product Release: https://openai.com/index/introducing-gpt-oss-safeguard/  
ROOST.tools press release: https://roost.tools/blog/a-new-milestone-for-open-source-safety-infrastructure-and-transparency/  
Reddit on open-weight v. open-source: https://www.reddit.com/r/opensource/comments/1mkqajs/how_can_gptoss_be_called_open_source_and_have_a/  
Elinor Ostrom & 8 rules for managing the Commons: https://tn.boell.org/en/2023/04/19/5-elinor-ostrom-et-les-huit-principes-de-gestion-des-communs  
OpenAI Developer Community: https://community.openai.com/t/fyi-to-stay-up-to-date-with-gtp-oss-changes-check-the-openai-github-repositories/1335535  
OpenAI usage policy: https://openai.com/policies/usage-policies/  
EU trusted flaggers: https://digital-strategy.ec.europa.eu/en/policies/trusted-flaggers-under-dsa  
EU AI Act: https://www.europarl.europa.eu/topics/en/article/20230601STO93804/eu-ai-act-first-regulation-on-artificial-intelligence
