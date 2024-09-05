

## 数据库操作
```bash

docker exec -it gunicorn python3 manage.py collectstatic --noinput 

docker exec -t mysql mysql -uroot -ptest@1q2w2e4R -e 'drop database adip;'
docker exec -t mysql mysql -uroot -ptest@1q2w2e4R -e 'CREATE DATABASE `adip` DEFAULT CHARACTER SET utf8 COLLATE utf8_general_ci;'
# 导出数据库
docker exec -i mysql mysqldump -uroot -ptest@1q2w2e4R adipv1 > adipv1.sql
# 导入数据库
docker exec -t mysql mysql -uroot -ptest@1q2w2e4R -e 'CREATE DATABASE `adipv1` DEFAULT CHARACTER SET utf8 COLLATE utf8_general_ci;'

## TODO 本项目需要的北荣；
docker exec -i mysql mysql -uroot -pAa123123 mango < mango_new_life.sql

```
