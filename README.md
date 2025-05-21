# 1.2. Understanding how it works.
"Paima's komputer: hey hey" akan di print lebih dahulu karena spawner.spawn hanya menambahkan task async ke antrean task. Spawner.spawn akan dijalankan dengan executor.run() yang ada setelah print "Paima's komputer: hey hey".

# 1.3. Multiple Spawn and removing drop
Ketika drop(spawner) tidak dipanggil, program akan hang dan harus menekan ctrl+c untuk menghentikan programnya. Hal ini dikarenakan executor mengasumsikan bahwa bisa saja task baru ditambahkan kapan pun.

