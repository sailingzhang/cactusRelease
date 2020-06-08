cactus是一个业余时间项目，主要集成了相关机器学习成果，形成一个开箱即用的服务。目前做成了docker, 提供grpc服务，方便其它开发语言（含web的js）直接访问。欢迎恰谈合作。  

目前支持  
(1)人脸检测，识别，追踪。  
(2)行人检测，追踪  
(3)车辆检测，追踪   
(4)车牌检测，识别，追踪。  
近期预期可以实现  
(1)交通道周边标志物识别，如 道跑，天空，建筑物，人行道，电杆等。  
(2)驾驶员行为识别，如， 是否在喝水，是否玩手机， 是否安全驾驶状态等。  
(2)人体部位检测。如眼，手，耳朵等。  
(3)文字检测,文字识别。  
中期预期可实现  
(1)语音，语言识别 

github地址：
https://github.com/sailingzhang/cactusRelease.git
docker hub 地址：
docker pull sailingzhang/cactus:latest 
简单的docker部署后即可在打开网页体验。

简单体验网址：
http://136.244.112.140:81/cactus/index.html
这个docker布部署在外网，因网速原因，视频分析体验不佳，建议本地部署。


机器学习定制：  
可定制特殊功能需求，满足不太常见的场景的机器学习任务。 对于小规模数据无需额外机器资源， 中等规模以上数据需提供自行提供GPU训练集群。  
可定制性能，平台需求，如集群，高并发，嵌入式（arm）平台  

欢迎推荐：  
推荐成功，二八分。  





Cactus is a project completed in spare time. It aims to integrate the ML achievement and form the Grpc Service In docker. 

Supported Currently:

(1)Face Detection, Face Recognition, Face Tracking. 
(2)Pedestrian Detection, Pedestrian Tracking.

(3)Vehicle Detection, Vehicle Tracking.

(4)License Plate Detection, License Plate Tracking.

Support in the near future. 

(1)The object detection and classification near the traffic route.

(2)the action of driver identification, like drinking, playing phone, driving in a  safe state, etc.

(3)The part of body detection, like the ear, knee, etc. 

(4)The text detection and identification. 

Support in the future. 

Automatic Speech Recognition. 

Github:

https://github.com/sailingzhang/cactusRelease.git

Docker hub:

docker pull sailingzhang/cactus:latest  

You could experience it after deploying quickly.  

Quick Experience: 

http://136.244.112.140:81/cactus/index.html
If you want to experience Analysing Video, please deploy it locally. 

ML Customization:

It can meet the needs of customization in an uncommon scene. 
No need for any other machine for little data.  Need supplied GPU for medium or big data. 
Satisfy the needs of performance optimization,  transplant to an embedded platform.

