# Dokumentasi Load Balancer Kafka Topics dengan Docker Compose

## Overview

Dokumentasi ini menjelaskan cara menggunakan Docker Compose untuk secara otomatis membuat load balancer.

## Requirements

- Docker dan Docker Compose terinstal pada sistem.
- Port `80` atau yang sesuai dengan konfigurasi dibuka agar bisa diakses dari luar vm.
- Menyesuaikan konfigurasi pada file `nginx.conf`

  - Pastikan pada bagian ini sudah diubah:

    ```conf
      upstream backend {
          server <ml1-ip>:<ml1-port>;
          server <ml2-ip>:<ml2-port>;
          server <ml3-ip>:<ml3-port>;
      }
    ```

## Deployment Steps

### 1. Menjalankan Docker Compose

Setelah konfigurasi selesai, jalankan Docker Compose untuk memulai proses pembuatan load balancer:

```sh
docker-compose up -d
```
