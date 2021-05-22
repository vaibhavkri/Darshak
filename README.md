## Darshak

# ngrok
./ngrok http 5005

# create new venv
source /opt/anaconda3/bin/activate
conda activate rasa-2-1-2

# install rasa and check
pip install rasa
pip list | grep rasa

# rasa x taking forever to install:
pip install rasa rasa-x -i https://pypi.rasa.com/simple --default-timeout=10000 --use-deprecated=legacy-resolver

# rasa run
rasa train
rasa shell

rasa run -m models --enable-api --cors "*" --debug

# pip update
python3 -m pip install -U pip

