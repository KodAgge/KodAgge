### Well met! 👋

Welcome to my GitHub! I'm currently pursuing a masters degree in Financial Mathematics at KTH in Stockholm, Sweden. I already have a bachelor's in Applied Mathematics + Industrial Engineering and Management at the same university. 

Even though I'm pursuing a degree in Financial Mathematics I also have a big interest in Data Analytics and Data Science, more specifically in Machine Learning. This is reflected in the repos you can find under my handle. Here is a selection of the projects I'm most proud of!

### ❓[Blackbox Feasibility Prediction](https://github.com/KodAgge/Feasibility-Prediction)❓

Working together with a fintech firm and three classmates we looked into the possibility of using Machine Learning to speed up their operations. The team within the firm we were working with had one main task: solving a constrained non-linear optimization problem using an evolutionary optimization algorithm called CMA-ES. However, there was one problem, deciding upon the feasibility of the solutions the algorithm suggested was computationally heavy. Our task was thus to see if Machine Learning could be used to filter out infeasible solutions. We took an explorative approach, testing a wide range of Machine Learning algorithms, supervised as well as unsupervised. Unfortunetaly, not method yielded useful results. We thinks this is mainly due to the evolutionary algorithm advancing towards the optimum in iterational steps through the large feature space (~4000 dimensions), which means that the classifiers needs to extrapolate.

![PCA](/images/PCA.gif)

### ✍️[Handwritten Mathematical Expressions to LaTeX](https://github.com/KodAgge/Img2Latex)✍️
As part of the final project in a Deep Learning course at KTH me and three classmates got the idea to of building a model that translates handwritten mathemtical expressions directly to LaTeX-code. This could save us a lot of time since manually entering equations into LaTeX is a very tedious task.

Looking into previous research we found that an Encoder-Decoder model consisting of a convolutional neural network (CNN) and a long short-term memory (LSTM) network would be most promising for our task. We thus constructed an Encoder consisting of a CNN with batch normalization and max-pooling and a Decoder consisting of a LSTM with a soft attention mechanism. For better performance beam search was used during prediction.

While the results weren't super promising for longer expressions the model performed well on some expression I wrote myself. Here are some examples!

![Result A](/images/result_a.PNG)
![Result B](/images/result_b.PNG)


### [Re-Implementation of Latent Dirichlet Allocation](https://github.com/Javigsv/LDA_AdML)

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
