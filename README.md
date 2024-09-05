# Yemeksepeti Customer Experience Metrics Analysis

## Overview
This project focuses on analyzing a dataset related to Customer Experience (CX) at Yemeksepeti, a leading online food and market ordering platform. The dataset contains 50,000 randomly selected restaurant orders from the first eight months of 2024, including key CX metrics across two primary customer service channels: the Contact (Operator) channel and the Self-Service channel.


## Dataset
Dataset field explanations:
+ **order_id**: primary key for the table and unique id for each order
+ **order_time**: day and time of the order (GMT+3)
+ **order_city**: province field of the delivery address
+ **order_area**: district field of the delivery address
+ **order_kitchen**: pre-defined kitchen group types for the order (i.e. Pizza)
+ **order_restaurant_id**: unique id of the restaurant
+ **order_size_TRY**: Amount of the order in Turkish Lira
+ **preffered_payment_method**: Preferred payment method chosen by user, can be Cash, Online Payment, Credit/Debit Card, Meal Card
+ **isSeamless**: If an order is seamless order, this field is 1, else 0. Boolean.
+ **isnotSeamless**: If an order is not a seamless order, this field is 1, else 0. Boolean.
+ **contact_reason_CSRLevel3**: A list of pre-defined complaints, types and detailes are provided in the Excel in different sheet.
+ **contact_reason_MainGroup**: CSR Level 3 complaints are grouped a higher complaint breakdown.
+ **isContact**: If a user contacted via live operator is 1, else 0. Boolean.
+ **isSelfService**: If a user is not seamless and not contacted via live operator, meaning Self -Service is used and value is 1, else 0. Boolean.
+ **ContactCSAT**: 1-5 scale points given by the user after Contact
+ **SelfServiceCSAT**: 1-5 scale points given by the user after Self-Service
+ **NPS-Q-Score**: 1-10 scale points given by the user about recommending Yemeksepeti to others. Used to calculate NPS.


## How to Use
Ortamı kurmak ve uygulamayı çalıştırmak için aşağıdaki adımları izleyin:
1. Clone the repository:
    ```bash
    git clone https://github.com/yemirvural/yemeksepeti-cx-metrics-analysis.git
    cd yemeksepeti-cx-metrics-analysis
    ```

2. Install the required Python libraries:
    ``` bash
    pip install -r requirements.txt
    ```

3. Open the Jupyter notebook and run the analysis:
    ```python
    jupyter notebook data-analysis.ipynb
    ```