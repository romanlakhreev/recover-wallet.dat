This Python script recovers deleted Bitcoin Core wallet.dat files from a disk image. It is particularly useful for Bitcoin Core wallets created between 2009 and ~2016 using the Berkeley DB (BDB) format.

The script works by searching for the BDB 1.85 magic bytes in the disk image. It reads the image in chunks and searches for the magic bytes within each chunk, effectively performing a raw search on the disk image.