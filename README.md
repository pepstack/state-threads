# state-threads

A copy from http://state-threads.sourceforge.net/


## build on rhel

cd state-threads/src/st-1.9/

make clean

make linux-debug (or linux-optimized)

cd obj/

## run test server

./server -l /var/log/st-server -b ip:port -i

in my case:

./server -b 192.168.56.101:8888 -i

Open a browser and then access the server URL: 192.168.56.101:888

## run test proxy

in my case:

./proxy -l 192.168.56.101:9000 -r 192.168.56.101:8888 -t 1 -X

Open a browser and then access to proxy URL: http://192.168.56.101:9000