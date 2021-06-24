#!/bin/bash
POOL=ethash.unmineable.com:3333
WALLET=TRX:TPrMLwJPz8kNfmxY1h5M41AhCeU5BQ7YHs
WORKER=$(echo $(shuf -i 1000-9999 -n 1)-Colab_Jay#im8m-ybvt)

chmod +x tuyulgpu
./tuyulgpu --algo ETHASH --pool $POOL --user $WALLET.$WORKER --ethstratum ETHPROXY
