# AI Methods Projects in Python

## English

This repository contains a set of Python-based projects developed for applying different Artificial Intelligence methods in practical scenarios.

The project includes three main implementations:

1. A 2D Pygame gravity runner game developed with the help of Generative AI
2. An Eight Queens solver using Hill Climbing with Random Restart
3. A machine learning classification workflow using Random Forest and KNN on the Breast Cancer Wisconsin dataset

The goal of this repository is to show how different AI-related concepts can be applied in code, including heuristic search, optimization behavior, game prototyping with GenAI assistance, supervised classification, model evaluation, and cross-validation.

---

## Project Overview

### 1. Gravity Runner Game with Pygame

This part of the project is a simple 2D endless runner game built with Python and Pygame.

The player controls a square that can switch between the floor and the ceiling by pressing the Space key. Obstacles move from the right side of the screen, and the player must avoid them by changing gravity direction.

The game was later improved with additional mechanics such as:

* Collectible stars
* Random player color changes
* Health/lives system
* Collectible hearts
* Restart mechanic
* Score tracking
* Difficulty increase based on score
* Simple UI improvements

This part helped me understand how Generative AI can support game prototyping, but also showed that generated code still needs to be reviewed, tested, and improved manually.

---

### 2. Eight Queens Solver with Hill Climbing

This part solves the Eight Queens problem using a Hill Climbing algorithm with Random Restart.

The Eight Queens problem requires placing eight queens on a chessboard so that no two queens attack each other. The board is represented as a one-dimensional list where each index represents a column and each value represents the row position of a queen.

The heuristic function calculates the number of queen conflicts. The algorithm repeatedly searches for a better neighboring board state. If it gets stuck in a local optimum, it restarts with a new random board.

The program runs multiple trials and records:

* Number of moves
* Number of random restarts
* Execution time
* Final board state
* Board visualization as image output

This part helped me understand how heuristic search works, why local optima are a problem, and how random restart can improve the success rate of hill climbing.

---

### 3. Machine Learning Classification with Random Forest and KNN

This part applies supervised machine learning on the Breast Cancer Wisconsin dataset using scikit-learn.

The dataset contains numerical features extracted from breast mass samples. The goal is to classify tumors as either malignant or benign.

The workflow includes:

* Loading the Breast Cancer Wisconsin dataset
* Splitting the data into training and test sets
* Applying standardization with `StandardScaler`
* Training a Random Forest classifier
* Training a K-Nearest Neighbors classifier
* Creating confusion matrices
* Predicting the class of a new instance
* Evaluating both models with 3-fold cross-validation

The project compares the performance of Random Forest and KNN using accuracy, precision, and recall.

This part helped me practice a full machine learning workflow: preprocessing, training, prediction, evaluation, and model comparison.

---

## Features

* 2D game development with Pygame
* Gravity switching mechanic
* Collision detection
* Score and lives system
* Collectible objects
* Hill Climbing algorithm for Eight Queens
* Random Restart strategy
* Heuristic conflict calculation
* Board visualization with Matplotlib
* Breast cancer classification with scikit-learn
* Random Forest and KNN model training
* Confusion matrix evaluation
* New instance prediction
* 3-fold cross-validation
* Accuracy, precision, and recall comparison

---

## Technologies Used

* Python
* Pygame
* Matplotlib
* scikit-learn
* Random Forest Classifier
* K-Nearest Neighbors Classifier
* StandardScaler
* Cross-validation
* Heuristic Search
* Supervised Machine Learning

---

## How to Run

### 1. Gravity Runner Game

Install Pygame:

```bash
pip install pygame
```

Run the game:

```bash
python main.py
```

Controls:

```text
SPACE - Switch gravity
R     - Restart after game over
```

---

### 2. Eight Queens Hill Climbing Solver

Install Matplotlib:

```bash
pip install matplotlib
```

Run the solver:

```bash
python 2ndquestion.py
```

The program prints trial results to the console and saves board visualizations as PNG files.

---

### 3. Machine Learning Classifier

Install required libraries:

```bash
pip install scikit-learn
```

Run the classifier:

```bash
python 4thquestion.py
```

The program prints:

* Random Forest confusion matrix
* KNN confusion matrix
* New instance predictions
* 3-fold cross-validation results

---

## What I Implemented and Learned

In this project, I worked with different Artificial Intelligence topics from both algorithmic and applied perspectives.

In the game development part, I practiced how Generative AI can be used for rapid prototyping. I also learned that AI-generated code should not be accepted blindly. The base code needed to be tested, extended, and adjusted to match the expected behavior.

In the Eight Queens section, I implemented a heuristic search solution. I practiced representing a problem state, calculating a heuristic value, generating neighboring states, and handling local optima with random restart.

In the machine learning section, I implemented a complete classification pipeline. I practiced data preprocessing, model training, prediction, confusion matrix interpretation, and cross-validation. Comparing Random Forest and KNN helped me understand that model performance depends on both the dataset and the evaluation method.

Main topics I practiced:

* Using Generative AI as a development assistant
* Building a simple interactive game with Pygame
* Implementing heuristic search
* Understanding local optima and random restart
* Solving the Eight Queens problem
* Visualizing algorithm results
* Preparing data for machine learning
* Applying standardization
* Training supervised classifiers
* Comparing machine learning models
* Evaluating models with confusion matrices and cross-validation

---

# Python ile Yapay Zeka Yöntemleri Projeleri

## Türkçe

Bu repository, farklı Yapay Zeka yöntemlerini pratik senaryolar üzerinde uygulayan Python tabanlı projeleri içermektedir.

Projede üç ana uygulama bulunmaktadır:

1. Generative AI desteğiyle geliştirilmiş 2D Pygame gravity runner oyunu
2. Random Restart destekli Hill Climbing algoritması ile Eight Queens çözümü
3. Breast Cancer Wisconsin veri seti üzerinde Random Forest ve KNN ile makine öğrenmesi sınıflandırması

Bu repository’nin amacı; heuristic search, optimizasyon davranışı, GenAI destekli oyun prototipleme, supervised classification, model değerlendirme ve cross-validation gibi yapay zeka konularının kod üzerinde nasıl uygulanabileceğini göstermektir.

---

## Proje Özeti

### 1. Pygame ile Gravity Runner Oyunu

Bu bölüm, Python ve Pygame kullanılarak geliştirilmiş basit bir 2D endless runner oyunudur.

Oyuncu, Space tuşuna basarak zeminden tavana veya tavandan zemine geçebilen bir kareyi kontrol eder. Sağ taraftan gelen engellerden kaçmak için doğru zamanda gravity yönü değiştirilmelidir.

Oyun daha sonra şu özelliklerle geliştirilmiştir:

* Toplanabilir yıldız nesneleri
* Oyuncu renginin rastgele değişmesi
* Can sistemi
* Toplanabilir kalp nesneleri
* Restart mekaniği
* Skor takibi
* Skora bağlı zorluk artışı
* Basit arayüz iyileştirmeleri

Bu bölüm, Generative AI’ın oyun prototipleme sürecinde nasıl yardımcı olabileceğini gösterdi. Aynı zamanda AI tarafından üretilen kodun doğrudan kabul edilmemesi, test edilmesi ve gerektiğinde manuel olarak iyileştirilmesi gerektiğini de gösterdi.

---

### 2. Hill Climbing ile Eight Queens Çözümü

Bu bölümde Eight Queens problemi, Random Restart destekli Hill Climbing algoritması ile çözülmektedir.

Eight Queens probleminde amaç, sekiz veziri satranç tahtasına birbirlerini tehdit etmeyecek şekilde yerleştirmektir. Tahta, tek boyutlu bir liste ile temsil edilir. Listedeki her index bir sütunu, değer ise o sütundaki vezirin satırını gösterir.

Heuristic function, vezirler arasındaki çakışma sayısını hesaplar. Algoritma sürekli olarak daha iyi komşu durumları arar. Daha iyi bir komşu bulunamazsa algoritma local optimum’a takılmış kabul edilir ve yeni rastgele bir tahta ile yeniden başlatılır.

Program birden fazla deneme çalıştırır ve şu bilgileri üretir:

* Hamle sayısı
* Random restart sayısı
* Çalışma süresi
* Final tahta durumu
* Tahta görselleştirmesi

Bu bölüm, heuristic search mantığını, local optimum problemini ve random restart yaklaşımının hill climbing başarısını nasıl artırabileceğini anlamamı sağladı.

---

### 3. Random Forest ve KNN ile Makine Öğrenmesi Sınıflandırması

Bu bölümde Breast Cancer Wisconsin veri seti üzerinde scikit-learn kullanılarak supervised machine learning uygulanmıştır.

Veri seti, meme kitlesi örneklerinden çıkarılmış sayısal özellikleri içerir. Amaç, tümörleri malignant veya benign olarak sınıflandırmaktır.

Uygulanan işlem akışı:

* Breast Cancer Wisconsin veri setini yükleme
* Veriyi training ve test setlerine ayırma
* `StandardScaler` ile standardization uygulama
* Random Forest classifier eğitme
* K-Nearest Neighbors classifier eğitme
* Confusion matrix oluşturma
* Yeni bir örnek için sınıf tahmini yapma
* 3-fold cross-validation ile modelleri değerlendirme

Bu bölümde Random Forest ve KNN modelleri accuracy, precision ve recall metrikleriyle karşılaştırılmıştır.

Bu çalışma, preprocessing, model eğitimi, tahmin, değerlendirme ve model karşılaştırma adımlarından oluşan tam bir machine learning workflow’unu uygulamamı sağladı.

---

## Özellikler

* Pygame ile 2D oyun geliştirme
* Gravity değiştirme mekaniği
* Collision detection
* Skor ve can sistemi
* Toplanabilir nesneler
* Eight Queens için Hill Climbing algoritması
* Random Restart stratejisi
* Heuristic conflict hesaplama
* Matplotlib ile tahta görselleştirme
* scikit-learn ile breast cancer classification
* Random Forest ve KNN model eğitimi
* Confusion matrix değerlendirmesi
* Yeni örnek tahmini
* 3-fold cross-validation
* Accuracy, precision ve recall karşılaştırması

---

## Kullanılan Teknolojiler

* Python
* Pygame
* Matplotlib
* scikit-learn
* Random Forest Classifier
* K-Nearest Neighbors Classifier
* StandardScaler
* Cross-validation
* Heuristic Search
* Supervised Machine Learning

---

## Çalıştırma

### 1. Gravity Runner Oyunu

Pygame kurulumu:

```bash
pip install pygame
```

Oyunu çalıştırma:

```bash
python main.py
```

Kontroller:

```text
SPACE - Gravity yönünü değiştirir
R     - Game over sonrası oyunu yeniden başlatır
```

---

### 2. Eight Queens Hill Climbing Çözümü

Matplotlib kurulumu:

```bash
pip install matplotlib
```

Çözüm dosyasını çalıştırma:

```bash
python 2ndquestion.py
```

Program deneme sonuçlarını konsola yazdırır ve tahta görsellerini PNG olarak kaydeder.

---

### 3. Machine Learning Classifier

Gerekli kütüphane kurulumu:

```bash
pip install scikit-learn
```

Classifier dosyasını çalıştırma:

```bash
python 4thquestion.py
```

Program şu çıktıları üretir:

* Random Forest confusion matrix
* KNN confusion matrix
* Yeni örnek tahminleri
* 3-fold cross-validation sonuçları

---

## Bu Projede Ne Uyguladım ve Ne Öğrendim?

Bu projede Yapay Zeka konularını hem algoritmik hem de uygulamalı taraftan ele aldım.

Oyun geliştirme bölümünde, Generative AI’ın hızlı prototipleme sürecinde nasıl kullanılabileceğini uyguladım. Bunun yanında AI tarafından üretilen kodun doğrudan yeterli olmadığını; test edilmesi, anlaşılması ve gerektiğinde manuel olarak geliştirilmesi gerektiğini gördüm.

Eight Queens bölümünde heuristic search çözümü implemente ettim. Problem durumunu temsil etme, heuristic değer hesaplama, komşu durum üretme ve local optimum durumlarını random restart ile aşma konularında pratik yaptım.

Machine learning bölümünde tam bir classification pipeline uyguladım. Veri ön işleme, model eğitimi, tahmin, confusion matrix yorumlama ve cross-validation adımlarını kullandım. Random Forest ve KNN karşılaştırması sayesinde model performansının veri setine ve değerlendirme yöntemine göre değişebileceğini gördüm.

Bu projede pratik yaptığım ana konular:

* Generative AI’ı geliştirme sürecinde yardımcı araç olarak kullanma
* Pygame ile basit interaktif oyun geliştirme
* Heuristic search algoritması uygulama
* Local optimum ve random restart mantığını anlama
* Eight Queens problemini çözme
* Algoritma sonuçlarını görselleştirme
* Machine learning için veri hazırlama
* Standardization uygulama
* Supervised classifier eğitme
* Makine öğrenmesi modellerini karşılaştırma
* Confusion matrix ve cross-validation ile model değerlendirme
