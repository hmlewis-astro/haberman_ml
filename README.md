# Haberman Cancer Survival Data with Machine Learning

The Haberman Dataset contains patient cases from a study conducted in the late-1950s and 1960s at the University of Chicago Billings Hospital, observing the long-term survival of patients who had undergone surgery for breast cancer. The notebooks in this repository present a **probabilistic model which predicts patient survival probability (for longer than 5 years after surgery), based on age, year in which the surgery was performed, and cancer spread (measured by the number of detected positive axillary nodes).** Note, data are not current and the sample size is relatively small, so we do not attempt to extrapolate the model to e.g., patients younger or older than the patients in the sample, or to patients undergoing surgeries today (>50 years after these data were collected).

## Results

A summary of the project and the results of the probabilistic model (as welll as all relevant generated figures) are presented in the [Final Report](Final_Report.pdf).

## Usage example

For a quick look at the dataset, download the data (``haberman.data.csv``), download and open the Jupyter Notebook with 
```sh
jupyter notebook haberman_analysis.ipynb
```
and run all cells (select "Cell" > "Run All" or press Shift+Return to run individual cells). This Notebook generates Figure 1 in the [Final Report](Final_Report.pdf). 

To train and run the model, download and open the Jupyter Notebook with
```sh
jupyter notebook haberman_final_model.ipynb
```
and run all cells (select "Cell" > "Run All" or press Shift+Return to run individual cells). When prompted, enter the age, year of operation, and number of positive axillary nodes for an imagnary patient whose long-term survival probability you'd like to check.  This Notebook also generates Table 1 and Figure 2 in the [Final Report](Final_Report.pdf). 

If you're interested in how the model was built, download and open the Jupyter Notebook with
```sh
jupyter notebook haberman_ml_build.ipynb
```
and run all cells (select "Cell" > "Run All" or press Shift+Return to run individual cells). When prompted, enter the age, year of operation, and number of positive axillary nodes for an imagnary patient whose long-term survival probability you'd like to check.

Please note, I am still very new at this whole *machine learning magic* thing, so most of the work in ``haberman_ml_build.ipynb`` is based on a tutorial by Jason Brownlee, [available at this website](https://machinelearningmastery.com/how-to-develop-a-probabilistic-model-of-breast-cancer-patient-survival/).

## Author

Hannah Lewis – hlewis@virginia.edu

Distributed under the MIT License. See ``LICENSE`` for more information.

[https://github.com/hmlewis-astro](https://github.com/hmlewis-astro)
