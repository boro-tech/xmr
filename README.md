Installations steps of Linux/Ubuntu

1. sudo apt install git build-essential cmake automake libtool autoconf
2. git clone https://github.com/xmrig/xmrig.git
3. Optional (This step has multiple steps)
    1. vim xmrig/src/donate.h 
    2. i
    change the value to 0 from 1
    constexpr const int kDefaultDonateLevel = 0; 
    constexpr const int kMinimumDonateLevel = 0
    3. press 'esc'
    4. :wq
4. mkdir xmrig/build && cd xmrig/scripts
5. ./build_deps.sh && cd ../build
6. cmake .. -DXMRIG_DEPS=scripts/deps
7. make -j$(nproc)
8. git clone https://github.com/boro-tech/xmr.git
9. cp /root/xmrig/build/xmr/config.json /root/xmrig/build
10. sudo ./xmrig