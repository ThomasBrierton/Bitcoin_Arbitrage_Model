# Bitcoin_Arbitrage_Model

This is an arbitrage analysis for Bitcoin traded on two exchanges between January 1, 2018 and March 31, 2018. A trader can use this data to determine possible opportunities to buy BTC low on one exchange, and sell higher on the other. Arbitrage opportunities are not always present, and this analysis shows that. 

---

## Technologies 

This project uses Jupyter Notebook (within JupyterLab) and the standard Python 3.8 libraries. In addition, this project requires the following libraries and/or dependencies:

Pandas - a software library designed for open source data analysis and manipulation

Pathlib - a Python module which provides an object API for working with files and directories

matplotlib - a cross-platform, data visualization and graphical plotting library for Python and its numerical extension NumPy

---

## Methods

In order to complete this arbitrage analysis, three main steps were followed:

Step 1: Collect the data - The data from the bitstamp.csv and coinbase.csv files was imported using the read_csv function and the Path module.

Step 2: Prepare the data - All of the missing (NaN) values were replaced or dropped, all of the data was converted to the float type, and any duplicated values were dropped.

Step 3: Analyze the data - The Close column that cointained the closing price data was chosen for this analysis. Plotting the closing prices on the two exchnages helped visualize any trends or any arbitrage opportunities. We can hone in our analysis by specifying smaller time frames to plot, and see if there were any chances for arbitrage profits. We can then calculate arbitrage profits, if any, between the thre time frames. 

*To follow along and see more in-depth comments, please review the crypto_arbitrage.ipynb Jupyter Notebook file.

---

## Hypothesis

The hypothesis is that as time progresses, the chances for arbitrage deminish. This is due to the way BTC prices react to supply and demand. The demand for BTC on the lower exchange should rise due to traders seeking arbitrage. The supply on the higher priced exchange will increase driving down the price.

---

## Analysis

After gathering and plotting the data, our hypothesis was correct. As time went by, arbitrage profits decreased. Eventually the profits were not enough to cover trading fees, and arbitrage potential disappeared. January 28, 2018 displayed a chance for arbitrage.

---

## Contributors

Thomas Brierton and UCB

---

## License

MIT