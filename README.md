# Docker Container Environment
Note:for testing 
1- Install Docker

```
cd bpm/latest
docker compose pull
docker compose up -d
```
## Restore datbase
### لايد من الانتظار دقيقة قبل تحميل قاعدة البيانات حتى يكون خادم قاعدة البيانات جاهزا
### استعادة قاعدة البيانات ربما تاخذ بعض الوقت حسب حجم قاعدة البيانات
```
sudo docker exec -it bpmdb sh init_db.sh
```

## للتاكد من عمل كل الخدمات
### لابد من الانتظار عدة ثواني قبل تشغيل الامر : حتى تكون كل الخدمات تم ربطها على قاعدة البيانات
```
docker ps # for check running services
```
<img width="925" alt="image" src="https://github.com/mas-soft/mas-dev-environment/assets/9312799/bd2b61e5-b4c9-4f5a-94e1-8417b8a2e6e9">

## للتشغيل 
```
http://localhost:1080
https://localhost:10443
```

## STOP Cluster
```
docker compose stop
```



## Restart Cluster
```
docker compose restart
```



## Drop Cluster
### جميع البيانات المسجلة داحل قاعدة البيانات سوف تحذف ولا يمكن الرجوع اليها
```
docker compose down
```

## Restart Servcie 
### على سبيل المثال الخزينة
```
docker restart cashbox
```
