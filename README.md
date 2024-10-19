# IBMZ-Datathon-24
# Code submission for IBMZ Datathon'24

# Problem Statement: Predicting Substance Use Risk Through Behavioral and Drug Usage Patterns
In today’s fast-paced world, increasing stress levels and easy access to substances have led to a growing public health concern surrounding drug abuse and addiction. Early detection and prevention of risky behaviors related to substance use are critical in promoting healthier lifestyles and reducing potential harm. However, predicting an individual’s risk of substance abuse is a complex task that involves multiple factors, including behavioral traits, personality characteristics, and past drug usage patterns.

Objective:
Develop a machine learning model that can predict an individual’s risk level for substance abuse based on their demographic information, personality traits, behavioral tendencies, and past drug usage patterns. The model will analyze these inputs and provide a risk score along with personalized advice to encourage healthier decision-making and preventive actions.

# Data and Inputs:
The solution leverages a dataset that includes:

Demographic Information: Age, gender, education, country, and ethnicity.
Personality Traits (NEO-FFI-R): Neuroticism, extraversion, openness to experience, agreeableness, and conscientiousness scores (0-10 scale).
Behavioral Traits: Impulsiveness (BIS-11) and sensation seeking (ImpSS) scores (0-10 scale).
Drug Usage Patterns: For 18 substances, including alcohol, cannabis, amphetamines, cocaine, nicotine, etc., users report their usage frequency (e.g., "Never Used", "Used in Last Month", "Used in Last Day").

# Solution:
The trained model utilizes a Random Forest Classifier wrapped inside a MultiOutputClassifier to handle multi-drug risk prediction. Users provide inputs on their drug consumption patterns and behavioral traits, and the model predicts their overall risk score on a scale of 1 to 10, where a higher score indicates a higher risk. The solution also outputs a behavioral factor score and a personality trait score, offering additional insights into users' risk tendencies.

# User Interaction:
The model takes input interactively through a series of questions related to demographics, personality traits, and drug usage.
Based on the user's input, it calculates and presents:
Behavioral Factor (out of 10)
Personality Trait Score (out of 10)
Drug Risk Factor (out of 10)
Personalized recommendations are provided based on the user's drug risk factor, with suggestions to seek help if necessary.

# Impact:
This tool can be used by healthcare professionals, rehabilitation centers, or as a self-assessment tool to proactively identify at-risk individuals, helping them take preventive actions or seek professional advice. By combining behavioral science and machine learning, the solution can contribute to combating the growing global issue of substance abuse.
