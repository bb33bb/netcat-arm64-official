# netcat-arm64-official
netcat-arm64-official

编译arm64命令：
```
wget -O config.sub 'https://git.savannah.gnu.org/gitweb/?p=config.git;a=blob_plain;f=config.sub;hb=HEAD'
chmod +x config.sub
LDFLAGS="-static" \
CFLAGS="-static" \
./configure \
--host=aarch64-linux-gnu \
--build=x86_64-linux-gnu \
--disable-shared \
--enable-static \
--enable-all-static
```
