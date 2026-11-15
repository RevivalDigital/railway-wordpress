FROM mariadb:12.3.3

# datadir dibuat di subfolder volume supaya folder "lost+found" bawaan
# volume tidak mengganggu inisialisasi database.
# bind-address=:: agar bisa diakses lewat private network Railway (IPv6/dual-stack).
CMD ["--datadir=/var/lib/mysql/data", \
     "--bind-address=::", \
     "--character-set-server=utf8mb4", \
     "--collation-server=utf8mb4_unicode_ci"]
