# cactusRelase

This is an application set of Machine  Learning which aims to apply the ML to our software easily.  It provided the GRPC interface so that you can run it in the network or integrate it into   your local software environment. More and more ML application interfaces would be included in the future. The following are supported currently.  
    
(1)rpc StockPredict1(StockPredict1Req) returns (StockPredict1Rsp);  
//this is an  auto trading  interface  for EurUs  by    Reinforcement  Learning. It's self-entertainment .  
(2)rpc FaceDetect_Mt(FaceDetectReq) returns (FaceDetectRsp);  
//this is face detecting by mtcnn.  
rpc FaceDetectAndIdentifyByPic_MFK(FaceDetectAndIdentifyByPicReq) returns (FaceDetectAndIdentifyByPicRsp);  
//this is face detecting and identifying by mtcnn, facenet,knn.  
rpc IdentifyPersonByThumbnails(IdentifyPersonByThumbnailsReq) returns (IdentifyPersonByThumbnailsRsp);  
//unimplemented.  



Install And Run From Docker:  
(1)  
docker pull sailingzhang/cactus:latest  
(2)  
docker container run --rm -p 8000:8000 -p:81:81 -p 8080:8080  -v /tmp/cactusshare:/app/share -it sailingzhang/cactus:latest  /bin/bash 


Test from Web:  
http://x.x.x.x:81/cactus/index.html

Run test  
(1)install opencv,grpc in python environment first. Python 3.6 recommended.      
cd cactusRelese/cactus/test (install from github)     or  cd /tmp/cactusshare/test(install from docker)  
python test.py xxxxx:8000 xxxxx.mp4  
  

Protocol:  
cactus.proto  is the proto file.   


configuration:  
cactus_configure.json is the configuration file. following are comments for some  elements.  
(1)"CactusServer":"127.0.0.1:8000"  
//listening address for such server.  
(2)"is_auto_classify":true  
//whether auto classify person.  
(3)        "train_directory":"share/facedetectandidentifybypictrain",  
        "identify_directory":"share/facedetectandidentifybypicidentify",  
//directory name for training and identifing.  

Note  
the Server for free can only live 30 minutes and has other limits. 
if you want  
to speed by using GPU,  
to speed by using OpenVino so that it could have a nice performance in the CPU environment,    
to work in the Embedded Software environment,    
to have a special requirement,   
please contact me.  email: sailingzhangflying@outlook.com.   Chinese or English could both be available.   

