---
type: slides
---

# Introduction to Decision Trees

<p align="center">
<img src="slide1.png" class="center" alt="slide" width="80%">
</p>
---

# What about cliché: Classroom spot:predictor of success?

<p align="center">
<img src="slide2.png" class="center" alt="slide" width="80%">
</p>

---

<p align="center">
<img src="slide3.png" class="center" alt="slide" width="100%">
</p>

---

<p align="center">
<img src="slide4.png" class="center" alt="slide" width="100%">
</p>

---
# Let's Draw a decision tree

<p align="center">
You have two minutes to draw a decision tree from the split presented before
</p>

---

# Let's Draw a decision tree

<p align="center">
<img src="slide6.png" class="center" alt="slide" width="60%">
</p>

---

# Gini Impurity

<p align="center">
<img src="slides7.png" class="center" alt="slide" width="60%">
</p>

---

# Giny Impurity for the front node

<p align="center">
<img src="slide8.png" class="center" alt="slide" width="60%">
</p>

---

# Giny Impurity for the left node

<p align="center">
<img src="slide9.png" class="center" alt="slide" width="80%">
</p>

---
# Choose your root

<p align="center">
<img src="slide10.png" class="center" alt="slide" width="80%">
</p>


---
# Grow the tree

<p align="center">
<img src="slide11.png" class="center" alt="slide" width="80%">
</p>

---
# Stop when Gini increase

<p align="center">
<img src="slide12.png" class="center" alt="slide" width="80%">
</p>

---
# Full Tree

<p align="center">
<img src="slide13.png" class="center" alt="slide" width="80%">
</p>

---
# Construction

* Start from the root node and compute Gini to choose the attribute
* Repeat the the same process from the leaf node
* Stop if the Gini impurity increase
* Stop when you reach the max depth
* Prune with a measure of residual_error/model_complexity

---
# Take away

* Supervised learning for classification or regression 
* Split the input space into cuboids  
* Split with to Gini impurity or Information Gain 
* Stop on Gini = automatic feature selection 

---
# What about numerical values ?

| AGE | h-homework/week | Pass test |
|----|----|-------|
| 20 | 0  | False |
| 25 | 2  | True  |
| 30 | 20 | False |
| 33 | 10 | False |
| 40 | 20 | True  |

- Sort the values
- Compute the average betweens adjacent instances
- Compute the Gini impurity for each average interval

<p align="center">
<img src="slide14.png" class="center" alt="slide" width="20%">
</p>

---

# What about categorical values ?

| Marker Color | Pass Test |
|-------|-------|
| Red | False |
| Black  | True  |
| Blue | True  |
| Red | False |

- Calculate the Gini impurity for each one as well as for each possible combination:
    - Blue
    - Black
    - Red
    - Black & Red
    - Blue & Red
    - Blue & Black

---

# Now, let's practice!
