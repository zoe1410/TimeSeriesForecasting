# Water-Level Forecasting

This research project compares a random forest with a one-dimensional convolutional neural network for forecasting water levels from past measurements. The accompanying paper describes the methodology and evaluation.

- [`RF.ipynb`](RF.ipynb) builds lag and calendar features for the random forest baseline.
- [`CNN_forecasting_timeseries.ipynb`](CNN_forecasting_timeseries.ipynb) builds input windows for a Conv1D model.

## Run the notebooks

The notebooks require the original `Waterlevel_Final.csv` dataset, which is not included. Place it in `data/` beside the notebooks. The data must include `Time` and `Waterlevel` columns.

```sh
python -m pip install notebook numpy pandas scikit-learn plotly matplotlib seaborn tensorflow
python -m notebook
```

Open the notebooks from the repository root and run the cells in order. The final Markdown cell in `RF.ipynb` records historical results from the original experiments.
