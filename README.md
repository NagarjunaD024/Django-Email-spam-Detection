# Django-Email-spam-Detection
In this repo, I had Integrated the machine learning model (Email Spam Detection) into a Django web application with a user friendly interface.

<div align="center">


![Language](https://img.shields.io/badge/Language-Python-blue)
![Framework](https://img.shields.io/badge/Framework-Django-092E20?logo=django&logoColor=white)
![Library](https://img.shields.io/badge/Library-Scikit--Learn-F7931E?logo=scikit-learn&logoColor=white)
![Database](https://img.shields.io/badge/Database-PostgreSQL-4169E1?logo=postgresql&logoColor=white)

</div>

---

## 🏗️ Project Architecture

This project follows the **MVT (Model-View-Template)** pattern, which is Django's implementation of the classic **MVC (Model-View-Controller)** architecture. 

| File | Component | Purpose |
| :--- | :--- | :--- |
| **`urls.py`** | **Controller (Router)** | Directs incoming web requests to the appropriate function in `views.py` based on the URL path. |
| **`views.py`** | **Controller (Logic)** | The core logic layer. It receives user input, interacts with the ML model, and decides which data to send back to the user. |
| **`models.py`** | **Model (Data)** | Defines the database schema. In this app, it can be used to store logs of scanned emails or user-submitted reports. |
| **`forms.py`** | **Data Validator** | Handles the HTML form logic, ensuring the text input is cleaned and validated before being passed to the ML detector. |
| **`templates/`**| **View (UI)** | The presentation layer. Contains HTML files that define how the spam detection results are displayed to the end-user. |

## Setup

1.  **Clone the Repository:**

    ```bash
    git clone [YOUR_REPOSITORY_URL]
    ```
 

2.  **Activate Virtual Environment:**

    ```bash
    python -m venv .venv
    .venv\Scripts\activate  # On Windows
    ```

3.  **Run Server:**

    ```bash
     cd ./spamDetection/ python manage.py runserver
    ```

## Result

![Spam](images/Stream-lit.png)

![Ham!](images/stream-lit-2.png)
