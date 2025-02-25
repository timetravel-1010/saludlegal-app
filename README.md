Start the database using Docker

```bash
sudo docker run --name saludlegal-db \
-p 1521:1521 \
-e ORACLE_PASSWORD=<YOUR-PASSWORD> \
-v path/to/saludlegal-app/database/init:/opt/oracle/scripts \
gvenzl/oracle-xe:21
```

Then run the initilize scripts

```bash
sudo ./database/setup.sh
```
