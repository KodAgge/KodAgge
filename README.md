# Well met! 👋

Welcome to my GitHub! I'm currently a consultant at Netlight within Data Science & Analytics. I have a master's degree in **Financial Mathematics** and a bachelor's in **Applied Mathematics + Industrial Engineering and Management**, both at KTH. 

Continue reading for a selection of the projects I'm most proud of!

### Languages and Tools:

[<img align="left" alt="Python" width="26px" src="https://github.com/KodAgge/KodAgge/blob/main/images/python.png" />]()
[<img align="left" alt="SQL" width="26px" src="https://github.com/KodAgge/KodAgge/blob/main/images/sql2.png" />]()
[<img align="left" alt="R" width="26px" src="https://github.com/KodAgge/KodAgge/blob/main/images/r.png" />]()
[<img align="left" alt="Matlab" width="26px" src="https://github.com/KodAgge/KodAgge/blob/main/images/matlab.png" />]()
[<img align="left" alt="PowerBI" width="26px" src="https://github.com/KodAgge/KodAgge/blob/main/images/powerbi.png" />]()
[<img align="left" alt="Qlik" width="26px" src="https://github.com/KodAgge/KodAgge/blob/main/images/qlik4.png" />]()
[<img align="left" alt="Excel" width="26px" src="https://github.com/KodAgge/KodAgge/blob/main/images/excel.png" />]()
[<img align="left" alt="VBA" width="26px" src="https://github.com/KodAgge/KodAgge/blob/main/images/vba.svg" />]()
[<img align="left" alt="Visual Studio Code" width="26px" src="https://github.com/KodAgge/KodAgge/blob/main/images/vsc.png" />]()
[<img align="left" alt="SAS" width="66px" src="https://github.com/KodAgge/KodAgge/blob/main/images/sas.png" />]()
[<img align="left" alt="Data Grip" width="26px" src="https://github.com/KodAgge/KodAgge/blob/main/images/datagrip.png" />]()
[<img align="left" alt="Google Sheets" width="19px" src="https://github.com/KodAgge/KodAgge/blob/main/images/googlesheets.png" />]()
<!-- [<img align="left" alt="Kuberneters" width="19px" src="https://github.com/KodAgge/KodAgge/blob/main/images/k8s.png" />]()
[<img align="left" alt="Grafana" width="19px" src="https://github.com/KodAgge/KodAgge/blob/main/images/grafana.png" />]()
[<img align="left" alt="Argo Workflow" width="19px" src="https://github.com/KodAgge/KodAgge/blob/main/images/argo.png" />]()
[<img align="left" alt="Docker" width="19px" src="https://github.com/KodAgge/KodAgge/blob/main/images/docker.png" />]()
[<img align="left" alt="PostgreSQL" width="19px" src="https://github.com/KodAgge/KodAgge/blob/main/images/postgresql.png" />]() -->


<br><br>

<!-- [![Top Languagess](https://github-readme-stats.vercel.app/api/top-langs/?username=KodAgge&layout=compact&hide=jupyter%20notebook&include_all_commits=true&count_private=true&title_color=000000)](https://github.com/KodAgge/)

<br> -->

## 📈 Reinforcement Learning for Market Making 📉

[![Readme Card](https://github-readme-stats.vercel.app/api/pin/?username=KodAgge&repo=Reinforcement-Learning-for-Market-Making&title_color=000000)](https://github.com/KodAgge/Reinforcement-Learning-for-Market-Making)

In collaboration with Skandinaviska Enskilda Baken (SEB), my classmate and I wrote our thesis about *Reinforcement Learning for Market Making*. Market making is the process of quoting buy and sell prices in a financial asset in order to provide liquidity and earn a profit on the spread. Setting these prices "correctly" is essential to drive volume, minimize risks and earn a profit &ndash; which historically has been done using analytical methods. However, derivation of optimal market making strategies is only possible when you make limiting and naïve assumptions on how markets work. There is thus an argument for using reinforcement learning to find better strategies since they do not depend on any of these assumptions.

Using two ways of modelling the market, we were able to use reinforcement learning to find market making strategies. In the first model, for which one can derive analytical strategies, we were able to use tabular Q-learning to find strategies that matched the analytically optimal strategies in performance. In the second model, which is significantly more sophisticated, we compared the performance of tabular Q-learning and Double Deep Q-Network (DDQN) and found that the latter was more suitable for this problem.

For more about our results, have a look at our **[thesis](https://kth.diva-portal.org/smash/record.jsf?pid=diva2:1695877)**.

_Below follows an illustration of a limit order book (LOB), a central concept of market making_.

<p align="center">
  <img src="/images/LOBIllustration.png" alt="An illustration of a limit order book" width="600"/>
</p>

<br>

## ✍️Handwritten Mathematical Expressions to LaTeX-code✍️

[![Readme Card](https://github-readme-stats.vercel.app/api/pin/?username=KodAgge&repo=Img2Latex&title_color=000000)](https://github.com/KodAgge/Img2Latex)

As part of the final project in a Deep Learning course at KTH me and three classmates got the idea to build a model that translates handwritten mathematical expressions directly to LaTeX-code. This could save us a lot of time since manually entering equations into LaTeX is a very tedious task.

Looking into previous research we found that an Encoder-Decoder model consisting of a convolutional neural network (CNN) and a long short-term memory (LSTM) network would be most promising for our task. We thus constructed an Encoder consisting of a CNN with batch normalization and max-pooling and a Decoder consisting of a LSTM with a soft attention mechanism. For better performance, beam search was used during prediction.

While the results weren't super promising for longer expressions, the model performed well on some expressions I wrote myself. Here are some examples!

<p align="center">
  <img src="/images/result_a.PNG" alt="Results A"/>
</p>
<p align="center">
  <img src="/images/result_b.PNG" alt="Results B"/>
</p>

<br>

## 📦Blackbox Feasibility Prediction📦

[![Readme Card](https://github-readme-stats.vercel.app/api/pin/?username=KodAgge&repo=Feasibility-Prediction&title_color=000000)](https://github.com/KodAgge/Feasibility-Prediction)

Working together with a fintech firm and three classmates, we looked into the possibility of using Machine Learning to speed up their operations. The team within the firm we were working with had one main task: solving a constrained non-linear optimization problem using an evolutionary optimization algorithm called CMA-ES. However, there was one problem, deciding upon the feasibility of the solutions the algorithm suggested was computationally heavy. Our task was thus to see if Machine Learning could be used to filter out infeasible solutions. We took an explorative approach, testing a wide range of Machine Learning algorithms, supervised as well as unsupervised. Unfortunately, no method yielded useful results. We think this is mainly due to the evolutionary algorithm advancing towards the optimum in iterative steps through the large feature space (~4000 dimensions), which means that the classifiers need to extrapolate.

_Below follows a gif of how the CMA-ES moves during its first 100 iterations, projected down to 3 dimensions using PCA_.

<p align="center">
  <img src="/images/PCA.gif" alt="PCAgif" width="750"/>
</p>

<br>

<!-- ## 📰Re-Implementation of Latent Dirichlet Allocation📰

[![Readme Card](https://github-readme-stats.vercel.app/api/pin/?username=Javigsv&repo=LDA_AdML&title_color=000000)](https://github.com/Javigsv/LDA_AdML)

  
In the final project of a course in Advanced Machine Learning, the task was to replicate the results of a famous paper within Machine Learning. Me and three classmates chose the 
[(2003) Blei et. al. paper Latent Dirichlet Allocation](https://github.com/Javigsv/LDA_AdML/blob/main/LDA%20paper.pdf) which introduced the LDA model; a model that was created for topic modelling in large corpora in order to find low-dimensional representations of documents while retaining statistical relationships useful for tasks relating to information retrieval.

Due to the model being intractible, one needs to use some kind of approximation technique. We thus used a Variational Inference - Expectation Maximization (VI-EM) algorithm.

We also looked at possibilities to extend upon the original paper. One thing we achieved was plotting topics' popularity over time. _Below follows such a plot for three topics._

<p align="center">
  <img src="/images/topicsovertime.png" alt="Topics over time" width="500"/>
</p>

<br> -->

## Wait, there's more!

While the projects above are my favourites, I still have more to show. Take a look at the following list if you want to learn more (some are unfortunately in Swedish):

>
> * **Deep Learning**
>   1. *[Implementing a Neural Network (NN) from scratch](https://github.com/KodAgge/NNs-in-matlab)*
>   2. *[Implementing a Convolutional Neural Network (CNN) from scratch](https://github.com/KodAgge/CNNs-in-matlab)*
>   3. *[Implementing a Recurrent Neural Network (RNN) from scratch](https://github.com/KodAgge/RNNs-in-matlab)*
>   4. *[Predicting the winning team in League of Legends based on team compositions](https://github.com/KodAgge/TeamCompositions)*
>
> * **Machine Learning**
>   1. *[Re-Implementation of Latent Dirichlet Allocation](https://github.com/Javigsv/LDA_AdML)*
>   2. *[Projects within Statistical Machine Learning](https://github.com/KodAgge/StatisticalMachineLearning)*
>   3. *[Other projects within Advanced Machine Learning](https://github.com/KodAgge/AdvancedMachineLearning)*
>
> * **Coding challenges**
>   1. *[Advent of Code 2022](https://github.com/KodAgge/Advent-of-Code-2022)*
>
> * **Numerical analysis**
>   1. *[Simulating the flight of a water rocket](https://github.com/KodAgge/WaterRocketSimulation)*
>
> * **Games**
>   1. *[An implementation of the classic "Hunt the Wumpus" game in pygame](https://github.com/KodAgge/Wumpus)*
>

<br>

[![KodAgge's GitHub stats](https://github-readme-stats.vercel.app/api?username=KodAgge&hide=issues&count_private=true&show_icons=true&title_color=000000)](https://github.com/KodAgge/) 

<!--
**KodAgge/KodAgge** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
