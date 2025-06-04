# AI-Based-Recommendation-System-Java


Company - Codtech IT Solutions
Name - Tanay Daata
Inter Id - CT04DL566
Domain - Java Programming
Duration - 4 Weeks
Mentor -  Mr. Muzammil Ahmed

# 🎯 Java Recommendation System Using Apache Mahout

## 📌 Project Overview

This project demonstrates how to build a **Recommendation System** using **Java** and **Apache Mahout**, a powerful machine learning library. The goal is to recommend **products or content** to users based on their past interactions or preferences, simulating real-world use cases such as e-commerce recommendations, movie suggestions, or content personalization.

The deliverable is a Java-based console application that utilizes **collaborative filtering algorithms** to suggest items. The application works with sample user-item preference data and generates recommendations for a given user.

---

## ✅ Features

* 🤖 Implements **user-based collaborative filtering**
* 📊 Supports **sample data input** via CSV files
* 🔄 Computes similarity using **Pearson Correlation**
* 📦 Uses **Apache Mahout** for recommendation engine logic
* ⚙️ Modular codebase with configuration flexibility
* 🧪 Easily testable with different datasets

---

## 📁 Project Structure

```
MahoutRecommender/
│
├── src/
│   └── Main.java                     # Entry point of the program
│
├── data/
│   └── preferences.csv              # Sample user-item preference dataset
│
├── pom.xml                          # Maven config for dependencies
│
├── README.md
└── .gitignore
```

---

## 🧰 Technologies & Libraries

* Java SE 8+
* Apache Mahout (for recommender engine)
* Maven (for dependency management)
* CSV file (as data model)

---

## ⚙️ How It Works

1. The program reads a CSV file (`preferences.csv`) containing user IDs, item IDs, and ratings.
2. It builds a **DataModel** using Mahout’s `FileDataModel`.
3. Computes **user similarity** using `PearsonCorrelationSimilarity`.
4. Forms a **neighborhood** of similar users using `NearestNUserNeighborhood`.
5. Uses Mahout’s `GenericUserBasedRecommender` to generate recommendations.
6. Outputs a list of top-N recommended items for a given user.

---

## 📊 Sample Input Format (`preferences.csv`)

```
1,101,4.5
1,102,3.0
2,101,4.0
2,103,5.0
3,102,2.5
3,104,4.0
```

Format: `userID,itemID,preferenceValue`

---

## 🧪 Sample Output

```
Recommended items for user 1:
Item ID: 103  | Score: 4.25
Item ID: 104  | Score: 3.75
```

---

## ▶️ How to Run

1. **Clone the Repository**

   ```bash
   git clone https://github.com/yourusername/MahoutRecommender.git
   cd MahoutRecommender
   ```

2. **Build the Project**

   ```bash
   mvn clean install
   ```

3. **Run the Application**

   ```bash
   mvn exec:java -Dexec.mainClass="com.example.recommender.Main"
   ```

4. **View Output in Console**

---

## 💡 Key Concepts Demonstrated

* **Collaborative Filtering**: Recommending items based on similar users' preferences.
* **Similarity Metrics**: Pearson correlation used to compute how closely two users relate.
* **Neighborhood-based Recommender**: Finds nearest neighbors and leverages their preferences.
* **Apache Mahout Integration**: Using high-level APIs for scalable recommendations.

---

## 🔄 Extensions & Ideas

* Add **item-based collaborative filtering**
* Connect to a **database** for dynamic user input
* Build a **REST API** for serving recommendations
* Integrate with a **web UI** using Spring Boot or Angular
* Support **real-time recommendation updates**

---

## 📌 Use Cases

* 🛒 E-commerce platforms for product suggestions
* 📽️ Streaming apps for movie or show recommendations
* 📚 E-learning platforms for course recommendations
* 📲 News or blog article personalization

---


