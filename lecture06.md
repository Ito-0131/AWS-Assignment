# 第6回課題

## CloudTrailイベント情報
イベント名：StopDBInstance

・含まれている内容  
"eventSource": "rds.amazonaws.com"
⇒リクエストが行われたサービスを示す。この場合、RDSに対してリクエストが行われた。

 "eventTime": "2024-11-03T09:45:09Z"  
⇒リクエストが完了した日時を示す。
Zulu Timeで「2024年11月3日09時45分09秒」にリクエストが完了したことを示している。日本時間に換算すると、9時間プラスされた「2024年11月3日18時45分09秒」にリクエストが完了したことを意味します。

"awsRegion": "ap-northeast-1"  
⇒ログインしたAWSリージョンを示す。

![image1](/images06/最後にAWSを利用した記録①.png)  

![image2](/images06/最後にAWSを利用した記録②.png)  

## CloudWatchのアラーム

通知方法：Amazon SNSを利用したメール通知)  
トピック名：ALB-Unhealthy-Targets-Alert  
![image3](/images06/作成したAmazon-SNS.png)

設定したアラームの詳細画面  
![image7](/images06/CloudWatchのアラーム詳細画面.png)

・Railsアプリケーションが使えない状態でのCloudWatchのアラート  
![image4](/images06/Railsアプリケーションが使えない状態でのCloudWatchのアラート.png)  

・Railsアプリケーションが使える状態でのCloudWatchのアラート  
![image5](/images06/Railsアプリケーションが使える状態でのCloudWatchのアラート.png)  

AWS利用料の見積もり  
URL：https://calculator.aws/#/estimate?id=1d2ea84cf711f2181ffe75ccc858ea8987e9e852

10月の利用料金  
![image6](/images06/AWS10月の利用料.png)  

・無料枠に収まっているかどうか  
⇒アカウント作成から時間が経っているため、無料枠ではない

### 第6回課題に取り組んでの感想
第5回課題と比べれば、楽に課題を進めることが出来た。  
AWSのサービスは、AWSを専門とするエンジニアになったとしても使い切れないのでは？と思うくらい、  
たくさんのサービスがあるので、書籍やWEBサイトなどを見つつ、課題とは関係の無いところも理解を深めていきたい。
