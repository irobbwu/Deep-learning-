## Assignment

+ 本次作業的資料是從行政院環境環保署空氣品質監測網所下載的觀測資料。
+ 希望大家能在本作業實作 linear regression 預測出 PM2.5 的數值。

#### Data Description
+ 本次作業使用豐原站的觀測記錄，分成 train set 跟 test set，train set 是豐原站每個月的前 20 天所有資料。test set 則是從豐原站剩下的資料中取樣出來。
    1. train.csv: 每個月前 20 天的完整資料。
    2. test.csv : 從剩下的資料當中取樣出連續的 10 小時為一筆，前九小時的所有觀測數據當作 feature，第十小時的 PM2.5 當作 answer。一共取出 240 筆不重複的 test data，請根據 feature 預測這 240 筆的 PM2.5。
+ Data 含有 18 項觀測數據 AMB_TEMP, CH4, CO, NHMC, NO, NO2, NOx, O3, PM10, PM2.5, RAINFALL, RH, SO2, THC, WD_HR, WIND_DIREC, WIND_SPEED, WS_HR。  

#### Kaggle & Submission Format
+ Link: https://www.kaggle.com/c/ml2020spring-hw1
+ 預測 240 筆 testing data 中的 PM2.5 值，並將預測結果上傳至 Kaggle
    1. Upload format : csv file
    2. 第一行必須是 id,value
    3. 第二行開始，每行分別為 id 值及預測 PM2.5 數值，以逗號隔開。
    
#### Description
+ 本次作業的資料是從中央氣象局網站下載的真實觀測資料，大家必須利用 linear regression 或其他方法預測 PM2.5 的數值。

+ 觀測記錄被分成 train set 跟 test set，前者是每個月的前 20 天所有資料；後者則是從剩下的資料中隨機取樣出來的。

+ train.csv: 每個月前 20 天的完整資料。

+ test.csv: 從剩下的 10 天資料中取出 240 筆資料。每一筆資料都有連續 9 小時的觀測數據，兒童學必須以此預測第十小時的 PM2.5。
  
#### Assignment Regulation
+ hw1.sh
    1. 請手刻實作 linear regression，方法限使用 gradient descent。
    2. 禁止使用 numpy.linalg.lstsq
+ hw1_best.sh

    不限定作法，但套件規定仍必須遵照期初公告。
    