Installations steps of Linux/Ubuntu

1. sudo apt install git build-essential cmake automake libtool autoconf
2. git clone https://github.com/xmrig/xmrig.git
3. mkdir xmrig/build && cd xmrig/scripts
4. ./build_deps.sh && cd ../build
5. cmake .. -DXMRIG_DEPS=scripts/deps
6. make -j$(nproc)
7. git clone https://github.com/boro-tech/xmr.git
8. cp /root/xmrig/build/xmr/config.json /root/xmrig/build
9. sudo ./xmrig