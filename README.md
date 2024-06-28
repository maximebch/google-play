# Unlocking App Success: A Data-Driven Exploration with Python

This project dives into a comprehensive dataset from the Google Play store to uncover the key factors that contribute to an app's success. Leveraging Python for data analysis, this notebook provides strategic insights and actionable recommendations for app developers and marketers.

## Table of Contents

- [Introduction](#introduction)
- [About the Dataset](#about-the-dataset)
- [Objectives of the Notebook](#objectives-of-the-notebook)
- [Step 1: Data Preparation](#step-1-data-preparation)
  - [1.1 Exploring the Dataset](#11-exploring-the-dataset)
  - [1.2 Format and Types of Variables](#12-format-and-types-of-variables)
    - [1.2.1 Correcting Values in a Row](#121-correcting-values-in-a-row)
    - [1.2.2 Genres: Separating Values](#122-genres-separating-values)
    - [1.2.3 Size: Converting KB to MB](#123-size-converting-kb-to-mb)
    - [1.2.4 Installs: Formatting and Converting to Integer](#124-installs-formatting-and-converting-to-integer)
    - [1.2.5 Type: Verification of the Classification](#125-type-verification-of-the-classification)
    - [1.2.6 Content Rating](#126-content-rating)
    - [1.2.7 App: Handling Duplicates](#127-app-handling-duplicates)
    - [1.2.8 Category and Genre: Overlap and Differences](#128-category-and-genre-overlap-and-differences)
  - [1.3 Checking for Outliers](#13-checking-for-outliers)
    - [1.3.1 Visualization of Outliers](#131-visualization-of-outliers)
    - [1.3.2 Outliers in Reviews](#132-outliers-in-reviews)
    - [1.3.3 Outliers in Installs](#133-outliers-in-installs)
    - [1.3.4 Outliers in Size](#134-outliers-in-size)
    - [1.3.5 Outliers in Price](#135-outliers-in-price)
  - [1.4 Handling Missing Values](#14-handling-missing-values)
    - [1.4.1 Converting "Varies with Device" Values as NaN](#141-converting-varies-with-device-values-as-nan)
    - [1.4.2 Identifying NaN](#142-identifying-nan)
    - [1.4.3 Imputation of Missing Values](#143-imputation-of-missing-values)
- [Step 2: Data Exploration](#step-2-data-exploration)
  - [2.1 Free Apps vs Paid Apps](#21-free-apps-vs-paid-apps)
  - [2.2 Categories and Genres Analysis](#22-categories-and-genres-analysis)
    - [2.2.1 Categories vs Rating](#221-categories-vs-rating)
    - [2.2.2 Genres vs Rating](#222-genres-vs-rating)
    - [2.2.3 Categories vs Price](#223-categories-vs-price)
    - [2.2.4 Genres vs Price](#224-genres-vs-price)
    - [2.2.5 Genres vs Size](#225-genres-vs-size)
  - [2.3 Rating vs Other Variables](#23-rating-vs-other-variables)
    - [2.3.1 Correlation Matrix](#231-correlation-matrix)
    - [2.3.2 Rating vs Reviews Size and Price](#232-rating-vs-reviews-size-and-price)
- [Conclusion](#conclusion)

## Introduction

When I came across this dataset from Kaggle, it felt like finding a hidden gem. As a data analyst focused on providing insights and solutions to marketing issues, I saw an opportunity to leverage this data and offer strategic recommendations on the kinds of apps that are most likely to succeed.

## About the Dataset

This dataset, sourced from Kaggle, contains scrapped data from the Google Play store, the app store for Android devices. It offers a comprehensive view of various aspects of mobile applications, ranging from user ratings and reviews to installation numbers and more.

## Objectives of the Notebook

In this notebook, I aim to dive deep into the dataset to unearth insights that could potentially guide app developers and marketers. My goal is to analyze the state of the Android apps market and identify the key factors that contribute to a successful app. By doing so, I hope to provide actionable recommendations for my company or clients who wish to build a new app and achieve success in the competitive app marketplace.
