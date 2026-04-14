# IITM Global Router for ICCAD 2026

This repository/container provides the **IITM Global Router** along with all necessary scripts to perform global routing on **ISPD 2025 / ICCAD 2026** testcases.

### 1. Load the Docker Image

```bash
docker load -i iitm_gr_iccad26.tar.gz
```
### 2. Start the container
```
docker compose -f docker-compose-iitm-gr.yml  up -d
```
### 3. Run the global router
```
docker exec -it iitm_gr /bin/bash
cd /media
./iccad_run_sqrtr.sh <cap_file_path> <net_file_path> <output_file_path>
```
