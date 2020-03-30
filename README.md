# state-threads
A copy from http://state-threads.sourceforge.net/


## build on rhel

cd state-threads/src/

make clean

make linux-debug (or linux-optimized)

cd obj/

## run test server

./server -l /var/log/st-server -b ip:port -i

Open a browser and then input in URL: http://ip:port
