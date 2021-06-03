## Darshak

# ngrok
./ngrok http 5005

# create new venv
source /opt/anaconda3/bin/activate
conda activate rasa-2-1-2

# install rasa and check
pip install rasa==2.4.3
pip list | grep rasa

# rasa x taking forever to install:
pip install rasa==2.4.3 rasa-x==0.38 -i https://pypi.rasa.com/simple --default-timeout=10000 --use-deprecated=legacy-resolver


# resolving rasa-x dependencies
pip uninstall attrs kafka-python questionary sanic-jwt ujson
pip install attes==19.3
pip install kafka-python==1.4.7 
pip install questionary==1.5.1 
pip install sanic-jwt==1.6.0 
pip install ujson==1.35

# rasa run
rasa train
rasa shell

rasa run -m models --enable-api --cors "*" --debug

# pip update
python3 -m pip install -U pip

