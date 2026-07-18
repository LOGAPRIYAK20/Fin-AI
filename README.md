# Fin-AI

AI Financial Wellness Bot
Problem Statement
Most people struggle to get a clear, personalized picture of their financial health. Budgeting apps show raw numbers, but rarely translate them into actionable insight — leaving users to figure out on their own whether they're actually doing well, overspending, or at risk. There's also no single place that combines budgeting, expense tracking, savings, investments, and bill reminders with a real assessment of overall financial wellness.
Solution
AI Financial Wellness Bot is a full-stack web application that gives users a secure, personalized dashboard to manage every aspect of their personal finances — and uses their real data to generate a Financial Wellness Score, tailored recommendations, and a conversational AI assistant that understands their specific financial situation.
Core Features
User Management

Secure registration and login with hashed passwords and session-based authentication
Personal profile (income, occupation, city, dependents) and custom financial goals

Financial Management

Budget Planner — set category-wise monthly spending limits
Expense Tracker — log and categorize real spending
Savings Tracker — record savings over time
Investment Advisor — log investments by type and risk level, with rule-based portfolio suggestions
Bill & EMI Reminders — track due dates and payment status
Financial Summary — real-time budget vs. expense comparison

AI & Analytics

Financial Wellness Score (0–100) — calculated from the user's actual budget-to-expense ratio and savings rate
Personalized Recommendations — generated from the same real-time financial signals
Credit Health Suggestions and Fraud Alerts — flags unusually large or repeated transactions
Insurance Guidance — suggestions based on savings thresholds
AI Chat Assistant — powered by a live LLM (Claude API), given real-time access to the logged-in user's actual budget, expenses, savings, and goals, so answers are grounded in their specific numbers rather than generic advice

Technical Architecture

Backend: Python, Flask, SQLAlchemy
Database: SQLite, with all financial tables (Budget, Expense, Saving, Investment, Reminder) linked to a central User table via user_id, ensuring complete data isolation between users
Frontend: Bootstrap 5, Chart.js for visual analytics, a dark-themed responsive dashboard
AI Layer: Anthropic Claude API integration for context-aware conversational assistance

What Makes It Novel
Unlike a standard budgeting tool, this project closes the loop between raw data and actionable insight: every number a user enters feeds directly into a wellness score, personalized recommendations, and a chatbot that can answer specific questions like "how am I doing this month?" using the user's real financial picture — not a static FAQ or keyword-based response.
