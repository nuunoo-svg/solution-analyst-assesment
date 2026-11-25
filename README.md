# Assesment Design

# Table of contents

**Chapter I**

  - [Architecture Overview](#architecture-overview)
  - [Architecture Component Specification](#architecture-component-specification)
  - [Backend Module Specification](#backend-module-specification)
  - [Technology Recommendation](#technology-recommendation)


  # Architecture Overview

  Tahap awal, backend dapat dibangun menggunakan Java Spring Boot dengan modular monolith. 
  Pendekatan ini lebih sederhana untuk dikembangkan dan dipelihara dibandingkan langsung menggunakan banyak microservices.
  ![architecture-overview]([https://github.com/nuunoo-svg/solution-analyst-assesment/blob/main/diagrams/architecture-overview.excalidraw](https://raw.githubusercontent.com/nuunoo-svg/solution-analyst-assesment/refs/heads/main/diagrams/architecture-overview.excalidraw))

  # Architecture Component Specification

  | Component                | Technology             | Responsibility                         | 
  | ------------------------ | ---------------------- | -------------------------------------- | 
  | Mobile Application       | Flutter                | User Interface Android and iOS         |
  | API Gateaway             | Spring Cloud Gateaway  | Routing, rate limit, authentication    | 
  | Backend                  | Java Spring Boot       | Business Logic                         | 
  | Database                 | PostgreSQL             | Save transactional and user data       | 
  | Cache                    | Redis                  | temporary session, caching, OTP        | 
  | Object Storage           | Compatible Storage     | ID and Selfie sotrage                  | 
  | Message Broker           | RabbitMQ/Kafka         | Asynchronous Processing                | 
  | Authentication           | JWT ++ Refresh Token   | Authentication and authorization       | 
  | Notification             | Email/SMS Provider     | sending Notification                   |
  | Payment Gateaway         | Payment Provider       | Installment and Disbursement Payment   |
    
