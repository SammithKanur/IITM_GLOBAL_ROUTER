# IITM Global Router for ICCAD 2026

### 1. Start the container
```
docker compose -f docker-compose-iitm-gr.yml  up -d
```
### 2. Run the global router
```
docker exec -it iitm_gr /bin/bash
cd /media
./iccad_run_sqrtr.sh <cap_file_path> <net_file_path> <output_file_path>
```
