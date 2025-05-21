# 1.2. Understanding how it works.
"Paima's komputer: hey hey" akan di print lebih dahulu karena spawner.spawn hanya menambahkan task async ke antrean task. Spawner.spawn akan dijalankan dengan executor.run() yang ada setelah print "Paima's komputer: hey hey".

