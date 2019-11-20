---
layout: post
title: Network Effects And Cascading Behaviour
header-includes:
   - \usepackage{amsmath}
---

In this section, we study how a infection propages through a network. We will look into two classed of model, namely decision based models and probabilistic models. But first lets look at some terminology used throughout the post.

**Terminology**
1. Contagion: What is spreading in the network, e.g., diseases, tweet, etc.
2. Infection: Adoption/activation of a node
3. Main players: Infected/active nodes, early adopters

# Decision Based Models
In decision based models, every nodes independently decides whether to adopt the contagion or not depending upon its neighbors. The decision is modelled as a two-player game between user and its neighbor and related payoffs. Hence a node with degree $$k$$ plays $$k$$ such games to decide its payoff and correspondingly its behavior.

## Single Contagion Model
There are two contagions $$A$$ and $$B$$ in the network and initially every node has behavior $$B$$. The payoff matrix is given as:
||A|B|
|A|a|0|
|B|0|b|

Lets analyze a node with d neighbors, and let p be the fraction of nodes who have adopted $$A$$. Hence the payoff for $$A$$ is $$apd$$ and payoff for $$B$$ is $$b(1-p)d$$. Hence the node adopts behavior $$A$$ if 
$$apd > b(1-p)d \implies p > \frac{b}{a+b} = q$$(threshold)

### Case Study: Modelling Protest Recruitment on social networks[]
Key Insights:
    - Uniform activation threhold for users, with two peaks
    - Most cascades are short
    - Successful cascades are started by central users

