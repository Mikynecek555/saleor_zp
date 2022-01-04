# Zaverecny projekt
-------------------
## Informace k projektu

![Snímek obrazovky 2022-01-02 201808](https://user-images.githubusercontent.com/47101285/147887512-73769e2a-df73-4be6-bfc7-24dd608e1548.png)


======
- docker-compose run api python manage.py dumpdata
- docker-compose run api python manage.py loaddata "location"
- 
 108  docker-compose up
  109  docker-compose run api python manage.py --saleor  loaddata testlll.json
  110  docker-compose run api python manage.py  loaddata --saleor testlll.json
  111  docker-compose run api python manage.py  loaddata --app saleor testlll.json
  112  docker-compose run api python manage.py  loaddata  'testlll'
  113  docker-compose run api python manage.py  loaddata  */testlll/*.json
  114  docker ps
  115* docker-compose run  python manage.py  dumdata
  116  docker-compose run api python manage.py  loaddata  
  117  docker-compose run api python manage.py  loaddata  --skip-checks test.json 
  118  exot
  119  docker-compose run api python manage.py  loaddata  -app saleor --skip-checks test.json 
  120  docker-compose run api python manage.py  loaddata  -*app saleor --skip-checks test.json 
  121  docker-compose run api python manage.py  loaddata  --app saleor --skip-checks test.json 
  122  docker-compose run api python manage.py  loaddata  --app saleor  test.json 
  123  docker-compose run api python manage.py  dumpdata  --app saleor  test.json 
  124  docker-compose run api python manage.py  dumpdata  product test.json 
  125  docker-compose run api python manage.py  dumpdata  products 
  126  docker-compose run api python manage.py  dumpdata  --exclude auth.permission --exclude contenttypes --indent 2 > db.json
  127  docker-compose run api python manage.py  loaddata  db.json
  128  docker-compose run api python manage.py  dumpdata  --indent=4 --all -e contenttypes -e sessions -e south > fulldb.json 
  129  docker-compose run api python manage.py  dumpdata  --natural --all -e contenttypes -e sessions -e auth.Permission > fulldb.json 
  130  docker-compose run api python manage.py  dumpdata  --natural -e contenttypes -e auth.Permission > fulldb.json 
  131  docker-compose run api python manage.py  dumpdata  -e contenttypes -e auth.Permission > fulldb.json 
  132  docker-compose run api python manage.py  loaddata  fulldb.json 
  133  docker ps
  134  docker-compose exec postgres backup
  135  docker-compose run postgres backup
  136  docker-compose run db backup
  137  docker exec -t db pg_dumpall -c -U postgres > dump_`date +%d-%m-%Y"_"%H_%M_%S`.sql
  138  docker exec -t saleor-platform_db_1 pg_dumpall -c -U postgres > dump_`date +%d-%m-%Y"_"%H_%M_%S`.sql
  139  ls
  140  cat dump_04-01-2022_11_52_09.sql 
  141  docker exec -t saleor-platform_db_1 pg_dumpall -c -U saleor -p saleor  > dump_`date +%d-%m-%Y"_"%H_%M_%S`.sql
  142  docker exec -t saleor-platform_db_1 pg_dumpall -c -U saleor -p saleor  > dump.json
  143  cat dump.json 
  144  docker exec -t saleor-platform_db_1 pg_dumpall -c -U saleor -P saleor  > dump.json
  145  cat dump.json 
  146  docker exec -t PGPASSWORD="saleor" saleor-platform_db_1 pg_dumpall -c -U saleor   > dump.json
  147  docker exec -t  saleor-platform_db_1  PGPASSWORD="saleor" pg_dumpall -c -U saleor   > dump.json
  148  cat dump.json 
  149  docker exec -t  saleor-platform_db_1  export PGPASSWORD="saleor" ;pg_dumpall -c -U saleor   > dump.json
  150  docker exec -t  saleor-platform_db_1  bash
  151  docker exec -t  saleor-platform_db_1  /bin/bash
  152  docker exec -it  saleor-platform_db_1  /bin/bash
  153  history
student@pcvyt3:~/mikes/saleor-platform/saleor/saleor$ docker exec -it  saleor-platform_db_1  /bin/bash
bash-4.4# history
    1  pg_dump
    2  PGPASSWORD="saleor" pg_dumpall -c -U saleor   > dump.json
    3  cat dump.json 
    4  cat dump.json |pgsql -U saleor
    5  psql -U saleor < dump.json 
    6  psql -U saleor < dump.json 
    7  pg_dumpall > dump.json 
    8  pg_dump > dump.json 
    9  pg_dump -U saleor  > dump.json 
   10  pg_dumpall -U saleor  > dump.json 
   11  psql -U saleor < dump.json 
   12  psql
   13  psql -u saleor
   14  psql -U saleor
   15  psql -U saleor < dump.json 
   16  exit
   17  history
bash-4.4# psql -U saleor
psql (11.1)
Type "help" for help.

saleor=# history
saleor-# 
select 'drop table "' || tablename || '" cascade;' from pg_tables;

- https://stackoverflow.com/questions/3327312/how-can-i-drop-all-the-tables-in-a-postgresql-database
