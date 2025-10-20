[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/oqKLEXJJ)
# 🎓 Ethical Admissions Algorithm Simulation

This repository is a classroom exercise exploring **ethics and fairness in algorithmic decision-making** — specifically in college admissions.

You’ll implement and reflect on how feature selection and weighting can impact fairness, transparency, and equity in automated systems.

---

## 🧩 Overview

You are part of the admissions committee for **Anonymous University**, located near Anonymous City.  
Due to a large number of applications, the committee decides to use an algorithm to help **rank and shortlist applicants**.

Your task:
- Decide which factors to include (GPA, test scores, extracurriculars, essays, recommendation letters, legacy status, income, etc.)
- Assign weights to each factor.
- Compare outcomes under two models:
  - **Blind model**: Ignores sensitive factors.
  - **Aware model**: Includes them intentionally to promote fairness (e.g., extra weight for first-gen or low-income applicants).

---

## ⚙️ How to Run

You can run the code on any online Java compiler (e.g. [Replit](https://replit.com/~) or [Programiz Java Compiler](https://www.programiz.com/java-programming/online-compiler))  
or locally via terminal:

```bash
javac Applicant.java Admissions.java Main.java
java Main
```

## Reflection

# Feature Selection & Design

I did not change the blind model at all. However, I did change the aware model. I removed legacy because that does not matter in my opinion. I changed the weight for firstGen applicants because I believe that those in this category are the most disadvantaged in general. I also changed the local weight, because those that are nearby should have a greater advantage than those from elsewhere. The reason for this is to benefit local community.

# Fairness & Outcomes

In the blind model, those that were academically less impressive were at a disadvantage. In the aware model, those that were, well, more disadvantaged in life had a greater advantage. The reason for this is to offset the disadvantage that some students have, giving them a "fairer" chance at getting the education they want. In my opinion, it depends on what university these systems are used for, but for a University like NMSU, I believe that the aware model is more fair. There are a lot of people who are not able to maintain a high GPA, study for good test scores, or participate in any extracurricular activities due to their circumstances. The aware model helps to offset this, allowing these people to receive a "fairer" chance.

# Transparency & Accountability

My algorithm seems pretty transparent. The only extra data it needs is the reasoning for specific Applicant parameter values such as Essay and Letter of Recommendation. Other than that, it would be relatively easy to explain to an applicant why they were rejected. Because of this, I would feel comfortable with this algorithm analyzing my applicaiton. It highly values academic success, but grants extra points for those that are disadvantaged and may not have been given the chance to succeed as much academically.

# Broader Implications

There are many, many risks, however. I said that I would be comfortable with my algorithm analyzing my own application, but in reality, it would need to go through much, much refinement to become truly reliable. In order to deal with real people and make decisions that affect real lives, any algorithm needs rigorous testing. Additionally, the algorithm should not be the end-all-be-all for applicant decisions. Multiple real humans need to evaluate the essay and letter of recommendation of a specific applicant before a decision can be made. Otherwise, unforseen bias may emerge. Although it is true that humans carry bias as well, an algorithm is much more vulnerable to these biases, and cannot do much to offset them. Additionally, since humans are naturally biased, and humans are the developers of these algorithms, then there is no way for any algorithm to ever be truly unbiased. 