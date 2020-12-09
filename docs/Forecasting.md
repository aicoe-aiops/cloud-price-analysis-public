# Cost Management : Forecasting

## _Aakanksha Duggal,  2020-November-12 v0.1.1-dev_

## Overview

_A brief summary of the project based on initial research and stakeholder meetings. To the best of your abilities, explain at a high level the stakeholders’ desired outcome for the project as well as the potential business value or impact this project will have if successfully completed._

1. **Situation and current issues:**

    In order to be able to make decisions about costs and resources, it is necessary to understand not only the current state of the resources, but also what will be the possible evolution of them. The customer should be capable of understanding the future evolution of the resources and costs if no action is taken, or if some action is taken on the source.

    The utility of the forecast can vary:

    *   Knowing the forecast for the end of the month can help operators to understand if everything remains as expected and take quick action if resources and costs get out of hand.
    *   End of quarter and end of year forecasts can help improve the budgeting  process and provide support for the financial department.

    Being able to use the forecast as a basis can improve the capability of cost management to show true costs when BOM rating needs to be done.

2. **Key Questions**
    1. End of month : Being able to show in the interface the forecast for the end of the month. The forecast should include a cone of confidence for better estimate, 1%, 5% (or similar).
    2. End of quarter : Being able to show forecasts for the end of the quarter.
    3. Cost forecasting for accounts and services : At the account level, being able to forecast overall costs for the account and for the services it uses.
    4. Application and service profiling : Identify services with a similar BOM and find parameters that can be used to describe them (i.e. identify services related to databases, and find performance for # of users, # of concurrent sessions, so it can be approximately sized).

3. **Approach:**  Current approach would be to use Linear Regression on the time-series data available. As the project and data-set grows, specialized methodologies like exponential smoothing or ARIMA can be used to make predictions of costs after each month or quarter.

4. **Impact:**

    *   **Manage Expenses :** Knowing the forecast for the end of the month can help operators to understand if everything remains as expected and take quick action if resources and costs get out of hand.
    *   **Improve Budgeting Process :** End of quarter and end of year forecasts can help improve the budgeting  process and provide support for the financial department.
    *   **Improve Capability of Cost Management :** Being able to use the forecast as a basis can improve the capability of cost management to show true costs when BOM rating needs to be done.

### A. Problem Statement:

_In as direct terms as possible, provide the “Data Science” problem statement version of the overview. Think of this as translating the above into a more technical definition to execute on._

The aim of this project is to start with a linear regression model that assumes a relationship between the input variable (month) and the predicted variable (Cost)on the existing time series data. Cost needs to be calculated from a linear combination of the input variable (month). The cost will be calculated on monthly and quarterly basis. And moving forward with the project, seasonality can be considered as a parameter and models like ARIMA can be tried out as well.

### B. Checklist for project completion

_Provide a bulleted list of the concrete deliverables and artifacts that, when complete, define the completion of the project._

1. Linear Regression on Cloud usage Data

## Resources

### Data Sets

*   Red Hat Cloud Spending data for last two months.

### Github

[https://github.com/aicoe-aiops/cloud-price-analysis-public](https://github.com/aicoe-aiops/cloud-price-analysis-public)
