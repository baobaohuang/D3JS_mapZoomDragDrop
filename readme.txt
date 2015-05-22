這是topojson 練習
先去政府的open data抓.shp圖資
http://data.gov.tw/node/7442
http://data.gov.tw/node/7441

檔案太大 所以把圖資拿去mapshaper 模糊化
並且轉成topojson檔

轉了以後 會有亂碼 所以用c# 轉碼big5 utf8
用codepage 那個範例去轉 
https://github.com/baobaohuang/codepageBig5UTF8

要注意的是轉了以後 有時候topojson 就讀不進去了
用parser 貼上去以後發現是 成功嶺 多了跳出碼 /
用codebeautify 去parser就好了
http://codebeautify.org/

最後加上room 和 drag drop 的method



註 .shp  ( ESRI Shapefile )

