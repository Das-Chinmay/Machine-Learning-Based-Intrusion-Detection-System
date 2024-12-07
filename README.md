# Machine-Learning-Based-Intrusion-Detection-System
This project demonstrates the effectiveness of machine learning in intrusion detection. The Random Forest model emerged as the best-performing model, achieving the highest accuracy while handling imbalanced data and feature complexity effectively.

This project is focused on building an Intrusion Detection System (IDS) using machine learning. The goal is to classify network traffic into two categories: normal or attack. To achieve this, we used the KDD Cup 1999 dataset, which contains network activity records with labels indicating whether the connection is normal or falls into one of several attack types. By training and evaluating multiple machine learning models, we aimed to identify the best-performing approach in terms of both accuracy and efficiency.

We chose this project because intrusion detection is a critical problem in cybersecurity, and machine learning offers promising solutions. The project also gave us the opportunity to practice essential skills, such as preprocessing data, working with machine learning models, and evaluating their performance using real-world metrics.

Dataset
The KDD Cup 1999 dataset was used for training and testing our models. It contains 41 features describing various attributes of network traffic, such as the protocol used (protocol_type), the service requested (service), and the connection status (flag). The target labels indicate whether the connection is normal or an attack.

There are four main attack categories:

DoS (Denial of Service): Overwhelms resources to make services unavailable.
Probe: Scans the network for vulnerabilities.
R2L (Remote-to-Local): Gains unauthorized access to a local machine.
U2R (User-to-Root): Escalates privileges to gain full control of a machine.
One challenge with this dataset is that it is highly imbalanced. Most records are labeled as DoS attacks, while others, such as R2L and U2R, are underrepresented. This imbalance made it critical to choose appropriate preprocessing and evaluation methods.

Methodology
We started by preprocessing the data to ensure it was ready for machine learning models. This involved encoding categorical features, removing redundant and low-variance features, and scaling numerical values for consistency. After preparing the data, we split it into training and testing sets to evaluate model performance on unseen data.

We trained five machine learning models:

Gaussian Naive Bayes
Decision Tree
Random Forest
Support Vector Machine (SVM)
Logistic Regression
For each model, we evaluated performance based on accuracy, test scores, and timing (both training and testing). These metrics helped us assess how well each model detected intrusions and how quickly they could process data, which is critical for real-time systems like IDS.
