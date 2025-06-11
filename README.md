Installations steps of Linux/Ubuntu

1. sudo apt install git build-essential cmake automake libtool autoconf
2. git clone https://github.com/boro-tech/xmr.git
3. mkdir xmr/build && cd xmr/scripts
4. ./build_deps.sh && cd ../build
5. cmake .. -DXMRIG_DEPS=scripts/deps
6. make -j$(nproc)
7. cp /root/xmr/config.json /root/xmr/build

Check the present working directory with 'pwd' it say '~/xmr/build#' ie it should be in build folder

8. sudo ./xmrig