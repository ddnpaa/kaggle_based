
# kaggleで共通して使うであろうソース

load_data.py  
→csvデータを読み込む

train_xgb.py  
→xgboostで学習を行う













# kaggle 教訓&メモ



①loggerは定期的に入れよう  
→どこでエラーが出ているかを確認できる上に、実行時間も出るため、どのくらい処理に時間がかかっているかもわかる。  
またkaggleにsubmitする際に残すメモにloggerの出力をそのままコピペするだけで、何をしたソースかわかる。

②モデルはほぼlightGBM,xgboost系の一強  
→kaggleでの上位争いは、**特徴量エンジニアリング**にかかっている。


③xgboostのパラメータの１つの学習率は初めは0.1で固定  
→これよりも下げてしまうと、処理に時間がかかってしまう。初めは特徴量エンジニアリングに時間を割くほうが有意義。  
ある程度特徴量エンジニアリングに見込みがなくなったら、学習率を0.01などに下げる。

___
その他　メモ  
  
[Takami_Sato様のチャンネル](https://www.youtube.com/channel/UCiECS_auJLNpFsvjTi1WuxQ)
  
[Markdownチートシート](https://gist.github.com/mignonstyle/083c9e1651d7734f84c99b8cf49d57fa)

