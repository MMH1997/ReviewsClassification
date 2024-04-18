# Madrid Metro Stations Reviews Classifier

Welcome to Madrid Metro Stations Reviews Classifier!!

Here, we provide the code used to conduct experiments aimed at comparing models for automatically distinguishing relevant from irrelevant reviews of Madrid Metro statins. 

## Content 
- **ComparingModels.ipynb**: This Jupyter Notebook contains the complete code for the experiments.

## Instructions
To filter only the comments belonging to the Airport or Hospital stations from the dataset, follow these steps:
1. Open the file `ComparingModels.ipynb`.
2. If you want to select only the reviews that pertain to 'Hospital' or 'Airport' stations, add one of the following lines:
    ```python
    df = df[df['Estación'].str.contains('Hospital')]
    ```
    or
    ```python
    df = df[df['Estación'].str.contains('Aeropuerto')]
    ```
    after
   ```python
   df = pd.read_excel('TODAS_ESTACIONES.xlsx')
   ```

5. Run the notebook to apply the filter.

## Data

Two randomly selected subsets of 1,000 comments each are available in the following files:

- **AllComments_1.xlsx**
- **AllComments_2.xlsx**

These files can be used as substitutes for `TODAS_ESTACIONES.xlsx` in case you want to work with smaller datasets.

## Results

The results obtained from all the experiments conducted for this work are summarized in the `Results.xlsx` file.

Happy exploring! 🚇📊
