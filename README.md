# Dokumentasi WS REST dengan Docker Compose

## Overview

Layanan berfungsi sebagai gateway untuk frontend.

## Requirements

- Docker dan Docker Compose terinstal pada sistem.
- Kafka sudah terdeploy.
- Layanan producer sudah terdeploy.
- Port `80` atau yang sesuai dengan konfigurasi dibuka agar bisa diakses dari luar vm.
- Pastikan environment variables sudah sesuai.

## Deployment Steps

### 1. Menjalankan Docker Compose

Setelah konfigurasi selesai, jalankan Docker Compose untuk memulai proses pembuatan layana:

```sh
docker-compose up -d
```
