---
marp: true
theme: uncover
style: |
    h1 {
        font-size: 50px;
        text-align: left;
    }
    h2 {
        font-size: 45px;
        text-align: left;
    }
    h3 {
        font-size: 40px;
        text-align: left;
    }
    section {
        font-size: 35px;
        /*text-align: left;*/
    }
    ul, ol {
        margin-left: 0;
        margin-right: auto;
    }
class: invert
paginate: true
#backgroundColor: #fff
---
# Hacking Machine Learning Systems
### Cédric Simal
---
# Motivation
### The current state of computer security
![height:400px](images/thisisfine.jpg)
http://gunshowcomic.com/648

---
# Plan
0. Why you should care
1. Security Framework
2. Common Attack types
3. Defenses

---
# All software can be hacked
![height:400px](images/tay.png)
https://knowyourmeme.com/memes/sites/tay-ai

---
# Why attack ML?
* Degrade model performance
* Find misclassified inputs
* Steal model parameters
* Steal training data

---
# Framework for attacks on ML 

![height:400px](images/framework.png)

[[Barreno et al.]](https://people.eecs.berkeley.edu/~adj/publications/paper-files/SecML-MLJ2010.pdf)


---
# Data Poisoning
![height:400px](images/data-poisoning.png)
[[Koh et al.]](https://arxiv.org/pdf/1811.00741.pdf)

---
# Adversarial Examples

![height:400px](images/adversarial_img_1.png)
openai.com

---
# Finding Adversarial Examples
* Whitebox : Fast Gradient Sign Method [[Goodfellow et al.]](https://arxiv.org/pdf/1412.6572.pdf)
* Blackbox: Surrogate model [[Papernot et al.]](https://arxiv.org/pdf/1602.02697.pdf)

---
# Attack Transferability
![height:400px](images/transferability.png)
[[Papernot et al.]](https://arxiv.org/pdf/1605.07277.pdf)

---
# Differential Privacy
![height:400px](images/privacy.png)
towardsdatascience.com

---
# Defense Strategies
* Reject On Negative Impact (RONI)
* Adversarial Training
* Ensemble methods
---
# Take home message
* Review your data
* Check your inputs
* Include Security at the design stage
---
# Learn more!
 Slides and sources at 
 https://github.com/csimal/ML-Hacking-Presentation
