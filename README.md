# 📈 Portfolio Insights
A stock price analysis and alerting tool that lets users search for stock data and create custom price alerts. Built with a modern, scalable backend and a clean, reactive frontend.

## 🧠 Project Overview

**Portfolio Insights** lets users:

- Search for stock price history by ticker symbol
- Visualize recent price trends in a dynamic chart
- Create alerts for when a stock goes _above_ or _below_ a custom price
- View, search, and delete alerts with a responsive UI

## 🛠️ Tech Stack

### Frontend
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css&logoColor=white)

### Backend

![Python](https://img.shields.io/badge/Python-2B5B84?style=for-the-badge&logo=python&logoColor=FFD845)
![Go](https://img.shields.io/badge/Go-1B2A33?style=for-the-badge&logo=go&logoColor=00ADD8)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-2B5B84?style=for-the-badge&logo=postgresql&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![psycopg](https://img.shields.io/badge/psycopg-2C5E83?style=for-the-badge&logo=postgresql&logoColor=white)


### Deployment

![AWS EC2](https://img.shields.io/badge/AWS%20EC2-FF9900?style=for-the-badge&logo=amazon-ec2&logoColor=white)
![AWS RDS](https://img.shields.io/badge/AWS%20RDS-527FFF?style=for-the-badge&logo=amazon-rds&logoColor=white)
![AWS Amplify](https://img.shields.io/badge/AWS%20Amplify-FF6144?style=for-the-badge&logo=aws-amplify&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-0db7ed?style=for-the-badge&logo=docker&logoColor=white)

### CI/CD

![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-1A1F2B?style=for-the-badge&logo=github-actions&logoColor=2088FF)
![Bash](https://img.shields.io/badge/Bash-1A1F2B?style=for-the-badge&logo=gnu-bash&logoColor=white)

### Linting
![lint-staged](https://img.shields.io/badge/lint--staged-1A1F2B?style=for-the-badge&logo=nodedotjs&logoColor=87cf30)
![Prettier](https://img.shields.io/badge/Prettier-1A1F2B?style=for-the-badge&logo=prettier&logoColor=F7B93E)
![ESLint](https://img.shields.io/badge/ESLint-1A1F2B?style=for-the-badge&logo=eslint&logoColor=4B32C3)
![Black](https://img.shields.io/badge/Black-1A1F2B?style=for-the-badge&logo=python&logoColor=white)


## 📂 Repositories

### `portfolio-insights-frontend`
A responsive React app built with Vite that allows users to search for stock tickers, visualize historical prices in an interactive chart, and manage price alerts. Layout and design styled with vanilla CSS, charts powered by Recharts, and notifications implemented with `react-hot-toast`.

_Deployment:_ Hosted on AWS Amplify with automatic deployments triggered by GitHub commits.

### `portfolio-insights-backend`
A FastAPI-based REST API that connects to PostgreSQL (via `psycopg`) for alert and user management, and communicates with the `market-service` microservice for live market data.

_Deployment:_ Deployed as a Docker container on AWS EC2, built and launched via GitHub Actions CI/CD pipelines and custom bash deployment scripts. Database is hosted on AWS RDS.

### `market-service`
A lightweight Go microservice that handles market data connectivity, retrieving historical stock prices and performing real-time alert validation through low-latency HTTP endpoints.

_Deployment:_ Compiled and deployed as a standalone binary on AWS EC2 using GitHub Actions and a custom shell-based deployment pipeline.

## 🚀 Features

- 🔍 Real-time ticker search with validation
- 📉 Historical price chart
- 🔔 Create stock alerts
- 🔄 Live refresh of alert display
- 🧼 Fully integrated linting/formatting workflow

## 🔍 Demo

https://portfolio-insights.jakubstetz.dev

API exposed at https://api.portfolio-insights.jakubstetz.dev

## 📄 License

MIT License
