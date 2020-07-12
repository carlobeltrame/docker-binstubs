FROM crisbal/torch-rnn:base

RUN echo '[ ! -z "$TERM" -a -r /etc/motd ] && cat /etc/motd' \
    >> /etc/bash.bashrc \
    ; echo "\
=============\n\
= torch-rnn =\n\
=============\n\
\n\
Preprocess the sample data:\n\
    python scripts/preprocess.py --input_txt data/input.txt --output_h5 data/input.h5 --output_json data/input.json \n\
\n\
Train\n\
    th train.lua -input_h5 data/input.h5 -input_json data/input.json -gpu -1\n\
\n\
Sample\n\
    th sample.lua -checkpoint cv/checkpoint_10000.t7 -length 2000 -gpu -1\n\n" > /etc/motd
