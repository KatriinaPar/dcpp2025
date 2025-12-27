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


## Improvements and recommendations

# Conclusion

# References
Hugging Face: https://huggingface.co/collections/openai/gpt-oss-safeguard  
OpenAI Product Release: https://openai.com/index/introducing-gpt-oss-safeguard/  
ROOST.tools press release: https://roost.tools/blog/a-new-milestone-for-open-source-safety-infrastructure-and-transparency/  
Reddit on open-weight v. open-source: https://www.reddit.com/r/opensource/comments/1mkqajs/how_can_gptoss_be_called_open_source_and_have_a/

Your content goes here. Please use [markdown](https://docs.github.com/fr/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github) for formating.
# title 1

## title 2

I love **EU**
