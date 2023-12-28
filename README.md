V1_V2_SMORE.ipynb: V1和V2的程式碼，預測的部分相同，只差在讀進去的檔案不同。最下方有將原始資料合併的程式碼，合併後的資料再使用SMORE做embedding。

V3_LSTM.ipynb: V3的程式碼，包含模型結構和後續預測。

V4_sort.ipynb: V4的程式碼，直接觀察此session歌曲出現次數，將出現多次的歌曲作為預測結果。

SMORE處理的指令如下:
```
./cli/hpe -train ts_all.txt -save hpe_all_ts_32.txt -undirected 0 -dimensions 32 -sample_times 300 -walk_steps 30 -negative_samples 30 -alpha 0.01 -thread 4
```
