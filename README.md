# ADK-Project
This is a adk web project.
Multi-Agent Fraud Detection System

This project implements a multi-agent system for fraud detection and analysis using Google ADK (google.adk).
It is designed to analyze uploaded financial transaction files (CSV/Excel) and detect suspicious patterns such as third-party payments and referee anomalies.

🚀 Features

Manager Agent (manager)

Central controller for all fraud-related analysis.

Routes requests to specialized sub-agents when needed.

Handles general fraud analysis queries and user interactions.

Payment Analysis Agent

Detects third-party payments (transactions paid by someone other than the customer).

Generates summary reports in markdown with:

Third-party flagged transactions.

Repeat third-party payers.

Provides deep-dive analysis per third party (total payments, total amounts, customer + branch mapping).

Referee Analysis Agent

Analyzes referee-related datasets to detect anomalies (e.g., mismatched records, duplicate entries).

(Extendable to more fraud domains).

File Handling Utilities

ensure_csv: Converts Excel to CSV automatically.

pre_processor: Cleans and normalizes uploaded transaction data.

auto_save_uploaded_file: Saves user-uploaded files and ensures consistent file handling.
