# Real-Time Fraud Detection Pipeline

## Background

Banks process millions of financial transactions every day across multiple payment channels, including **Credit Cards, ATMs, POS terminals, and UPI**. Alongside these transactions, fraud intelligence is continuously received from internal fraud teams and external security partners. Since fraudulent activity can spread rapidly, even a small delay in detection may result in significant financial losses and a poor customer experience.

---

## Problem Statement

Building an effective fraud detection system presents several challenges:

- Fraudulent transactions must be identified and flagged within **seconds**.
- Fraud indicators originate from multiple real-time and batch sources, including:
  - Live transaction streams
  - Fraud watchlists
  - Customer master data
  - Merchant reference data
- Traditional batch-processing systems cannot react quickly enough to prevent fraudulent transactions before they are completed.

---

## Solution

This project implements a **real-time fraud detection pipeline** using modern streaming technologies.

The pipeline:

- Ingests live credit card transactions through **Apache Kafka**.
- Continuously processes fraud watchlist updates from **JSON files**.
- Enriches transaction streams with customer and merchant reference data.
- Performs **streaming joins**, **window-based analytics**, and **rule-based fraud detection**.
- Generates real-time fraud alerts and powers operational monitoring dashboards for rapid investigation and response.