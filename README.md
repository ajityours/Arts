# FoodSaver AI: Smart Pantry & Waste Minimizer

Final project for the Building AI course

## Summary

FoodSaver AI is a computer vision and optimization tool designed to track household groceries. By identifying items via photos and analyzing expiration dates, it suggests recipes to use up food before it spoils, significantly reducing household waste and saving money.

## Background

Food waste is a global crisis with significant economic and environmental impacts.
* **The Problem:** 1/3 of all food produced globally is wasted, with households being a major contributor.
* **Frequency:** The average person forgets what is in the back of their fridge, leading to expired goods weekly.
* **Motivation:** My goal is to make sustainable living effortless by using AI to bridge the gap between "what I have" and "what I can cook."

## How is it used?

The solution is used in a home kitchen environment. 
1. **Input:** The user takes a photo of their grocery receipt or the inside of their fridge.
2. **Processing:** The AI identifies items and estimates shelf-life.
3. **Action:** The user receives a notification: "Your spinach expires in 2 days. Try making Creamy Spinach Pasta tonight!"

The needs of busy professionals and families are prioritized by keeping the interaction time under 30 seconds.

<img src="https://upload.wikimedia.org" width="300">

## Data sources and AI methods
The project relies on a combination of image recognition and recommendation algorithms.
* **Image Data:** [Food-101 Dataset](https://www.kaggle.com) for identifying ingredients.
* **Methods:** 
    * **Convolutional Neural Networks (CNN):** To classify items from images.
    * **Filtering Algorithms:** To match available ingredients with a recipe database.


| Tech Layer | Method |
| ----------- | ----------- |
| Recognition | CNN (MobileNetV2) |
| Logic | Rule-based expiration tracking |
| Recommendation | Content-based filtering |

## Challenges

* **Project Scope:** It does not solve the issue of food quality (e.g., it can't "smell" if milk has gone sour prematurely).
* **Ethics:** Data privacy is a concern; the AI should only process images of food items and ignore any faces or personal information captured in the background.

## What next?

The project could grow by:
* Integrating with grocery store APIs for automatic digital receipt syncing.
* Collaborating with nutritionists to provide health-focused meal plans.
* I would need a partner with expertise in mobile app development (Flutter/React Native) to make this a portable tool.

## Acknowledgments

* Inspired by the "Zero Waste" movement and the University of Helsinki's Building AI course.
* [Food-101 Dataset](https://data.vision.ee.ethz.ch) by Bossard et al.
* Reaktor Innovations for the project template.
