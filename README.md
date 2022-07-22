# Minio

```bash
docker run --rm \
  -p 9000:9000 \
  -p 9001:9001 \
  -e "MINIO_ROOT_USER=AKIAIOSFODNN7EXAMPLE" \
  -e "MINIO_ROOT_PASSWORD=wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY" \
  quay.io/minio/minio server /data --console-address ":9001"
```
API: http://172.17.0.4:9000  http://127.0.0.1:9000 

Console: http://172.17.0.4:9001 http://127.0.0.1:9001 

___________________________________________
```bash
pip3 install minio

python3

from minio import Minio
minioClient = Minio('play.min.io:9000',
access_key='Q3AM3UQ867SPQQA43P2F',
secret_key='zuf+tfteSlswRu7BJ86wekitnifILbZam1KYY3TG',
secure=True)
print(minioClient)                  
```
