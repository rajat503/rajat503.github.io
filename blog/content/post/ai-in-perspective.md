+++
date = "2017-06-18T00:32:40+05:30"
draft = false
title = "Putting AI in Perspective"

+++
An attempt to collect thoughts on AI and where it might be headed.
<!--more-->

## Background
Artificial Intelligence has been on the rise lately - all major technology companies are heavily investing in it, a lot of papers are being published daily on arXiv, tech blogs are sensationalizing it, most computer science undergrads want to study it. Amidst all this, it has been a year that I've been looking at topics in deep learning and I thought it might be worthwhile to try to summarize the current scenario with its limitations and the future one can expect in broader terms.

## Themes
### Supervised data
We have been able to leverage big datasets (thanks to the internet) and more compute power to train better algorithms. Deep models have performed extremely well on image data and more recently on NLP tasks. The accuracies on existing benchmarks improve every year and we can expect this trend to continue in computer vision (for videos) as well as NLP. Most improvements are and will continue to be because of the research that goes into building better models that learn from supervised data. Better and more complex supervised datasets will be built as we start performing well on existing ones.

However, gathering a large amount of supervised data is costly. The next logical step is to come up with unsupervised algorithms or models that can learn from a lesser amount of data - like humans do. In the future, we can expect a lot more research to go into this but little can be said about the probability of a breakthrough similar to supervised learning.

### Narrowness
Most of the supervised models perform well only on narrow tasks. We have been able to build agents that achieve human level performance on one task or similar tasks. While better performance on one task might be useful to build real world applications, it should not be confused with a breakthrough in AI, as the media does (Google's Neural Machine Translation learning its own language or AlphaGo, anyone?). It is just software performing a task better and is far from any general artificial intelligence. Andrej Karpathy talks more about this in his blog post <a href="https://medium.com/@karpathy/alphago-in-context-c47718cb95a5" target="_blank">AlphaGo, in context</a>.

### Hardware
Building supervised models that work on narrow tasks presently require a lot of computational power. The rise in deep learning was possible because of the advances in GPU computing and Google recently came up with TPUs - ASIC for machine learning. Moving forward, we can expect more development in ASIC architectures for gains in computing power and energy efficiency for both mobile and server class machines.      

### Transition to Cloud
Most companies which have the advantage of data and resources to fund AI research have started to build cloud platforms for machine learning (Machine Learning as a Service?). This is also true for research groups which win the benchmark challenges every year. Moving to the cloud is a welcome change for multiple reasons:

1. End devices can get away with lesser computational power by off-loading compute intensive tasks to the cloud. This reduces costs and energy requirements for the end devices while not compromising the quality of the model (smaller model for mobile devices).

2. A larger group of developers can integrate and use AI in their apps without learning the underlying concepts of AI.

3. Perhaps the most important area impacted by the cloud is Internet Of Things and Personal Computing. As more devices around us connect to the internet, AI on the cloud can be super useful in personalizing experiences across devices and making devices work in collaboration. Assistants and smart homes are just an example and we can expect more integration in the future.

Cloud, however, comes with the cost of network latency and we need faster and more reliable networks for this model to realize its full potential. Also, there will be scenarios where real-time on device processing cannot be avoided.

### Software
1. The integration of algorithm-driven design with a data-driven design. This equips modern apps with AI capabilities making them more useful. (I guess that is what Google means by AI first, in some sense.)

2. Libraries like TensorFlow and PyTorch which abstract the hard engineering involved in making AI work on different hardware and allow developers and researchers to focus on AI instead of system challenges.

These libraries can be seen as providing lego blocks for machine learning. In the future, we can expect these lego blocks to get more complex and standardized - like a full deep network for vision classification. This would happen once we start to fix architectures for standard tasks.

## Challenges
### Adversarial Examples
One of the open problems in machine learning that people often pay less attention to is of generating examples that are capable of fooling the models. OpenAI made a <a href="https://blog.openai.com/adversarial-example-research/" target="_blank">blog post</a> about it a while back discussing the problem in detail.

### Privacy
There is always a big debate around using user data for machine learning and it could be quite a while before this is settled.

### Data Leverage
Currently, bigger companies have the advantage of data and startups cannot be happy about this. While democratizing AI through publishing research is awesome, something needs to be done in the domain of data as well. Smaller companies would find using AI cloud services very restrictive.

### Jobs and Advanced AI
An even bigger concern about the development of AI is of jobs being automated by machines. While that is true, this discussion would be incomplete without considering the opportunities that will be created by AI. Any automation allows an individual or an organization to do and achieve more which in turn opens up more opportunities in the future. A lot of jobs have been automated by computers today, but that automation paved way for growth which created more jobs and industries which were previously unthinkable. I'm glad that governments and independent bodies are considering this to chart a map for a sustainable future.

## Conclusion
The buzz around artificial intelligence is huge mainly because of how people and the media choose to sensationalize it. I think it would be more sane and reasonable to view these advances as software getting better at tasks which we wished computers could do. This would mean technology complementing and not competing with humans for a better future.
