### create airflow group and add user to it

```bash
sudo groupadd -g 50000 airflow
sudo usermod -aG airflow $USER

# check if user is added to group
groups $USER
```
