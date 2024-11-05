# Contextual Multi-Armed Bandit for News Article Recommendation

Implementing a Contextual Multi-Armed Bandit (MAB) solution using the Upper Confidence Bound (UCB) algorithm for recommending news articles. The objective is to maximize the average time users spend on recommended articles by leveraging user context to make recommendations.

## Overview

The Contextual Multi-Armed Bandit model treats each article as an arm in the bandit. The system records user engagement data (reward) as time spent on an article, along with contextual information (time of day, user age group, and device type). These contextual features are used to select and recommend articles that are likely to engage the user.

This method uses a UCB adjusted for contextual relevance, making recommendations that are both exploratory and contextually relevant.

## How It Works

1. **Contextual Data**: The model considers each article’s contextual information and the user’s current context to compute relevance.
2. **UCB with Contextual Adjustment**: Each article is evaluated based on its expected reward, confidence interval, and contextual relevance.
3. **Simulated User Interaction**: For each recommendation, user engagement (reward) is simulated, factoring in how well the recommendation aligns with the user’s context.

## Features

- **Context-Aware UCB**: Adjusts the UCB algorithm to factor in article-user context relevance, improving recommendation personalization.
- **Dynamic Rewarding**: Calculates rewards based on time spent per article and contextual alignment.
- **Scalable Architecture**: The code can be scaled up to handle more articles and more relevant contextual data.

## References

- [Heewon-Hailey's GitHub - Multi-Armed Bandits for Recommendation Systems](https://github.com/Heewon-Hailey/multi-armed-bandits-for-recommendation-systems)
- [Yubin-Cho's GitHub -  Multi-armed Bandits for Recommendation System] (https://github.com/yubin1219/multi_armed_bandits_recommendation_system)
- Sutton, R. S., & Barto, A. G. (2018). Reinforcement Learning: An Introduction.
