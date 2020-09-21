ML_Contributions
==============================

This analysis aims to predict donor behavior amongst first-time donors for a performing-arts nonprofit organization in the US. This project will use a combination of classification and regression algorithms to predict the following:
    1) which customers are most likely to make a tax-deductible donation in conjunction with a ticket order; 
    2) which customer will make a tax-deductible conrtibution with a subsequent order; or
    3) the number of days following their first order that a customer may make a tax-deductible donation.
    
In addition, we'll create a model to see how the internal dimensions of a customer's ticket order may be able to predict their tax-deductible "lifetime value". This last target was an impromptu idea to see how transactional behavior might influence philanthropic activity.

The concepts that informed this project revolve around the idea of targeted messaging or offers, such as discounted donation benefits. It would also be possible to couple this analysis with similar prediction models to issue an offer for discounted tickets, merchandise, or donor benefits based on a given customer's propensity for building affinity in one of those ways, as predict by the dimensions of their online order activity.

The conclusions from this project are as follows:
<ol>
    <li>Predicting a donation from a first-time customer would require parameters outside of the scope of the ticket order itself. Possible sources that could improve prediction would be demographic- and income information based on the customer's ZIP code, or performing a "wealth screening" prior to the customer completing their order.</li>
    <li>It is possible to predict which customers will make a donation following their first order, plus we can predict a roughly 6-month window during which that donation is most likely to take place. We can then created a targeted appeal for customers who fall into that "sweet spot". At the same time, we can look at other new customers who are unlikely to make a donation as a potential target for other affinity offers.</li>
    <li>As a matter of curiousity, I also looked at the relationship between lifetime giving, which is one of the most secure forms of revenue and customer affinity, to ticket behavior, to verify whether or not there is a strong correlation for a given customer.</li>
    </ol>

Project Organization
------------

    ├── LICENSE
    ├── Makefile           <- Makefile with commands like `make data` or `make train`
    ├── README.md          <- The top-level README for developers using this project.
    ├── data
    │   ├── processed      <- The final, canonical data sets for modeling.
    │   └── raw            <- The original, immutable data dump.
    │   │
    ├── models             <- Trained and serialized models, model predictions, or model summaries
    │
    ├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
    │                         and a short description, e.g. `1.0- Data Pre-Processing`.
    │
    ├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
    │   └── figures        <- Generated graphics and figures to be used in reporting
    │
    ├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
    │                         generated with `pip freeze > requirements.txt`
    |
    |──environment.yml     <- The .yml environment file from Conda.
    │
    └── tox.ini            <- tox file with settings for running tox; see tox.readthedocs.io


--------

<p><small>Project based on the <a target="_blank" href="https://drivendata.github.io/cookiecutter-data-science/">cookiecutter data science project template</a>. #cookiecutterdatascience</small></p>
