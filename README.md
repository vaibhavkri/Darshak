# Darshak
 
# rasa x taking forever to install:
pip install rasa rasa-x -i https://pypi.rasa.com/simple --default-timeout=10000 --use-deprecated=legacy-resolver

# python 3.8 venv
source darshak_venv/bin/activate
cd Darshak

# rasa run
rasa train
rasa shell

# pip update
python -m pip install -U pip

# install ngrok (for deployment globally outside on the internet)
brew install --cask ngrok

# install homebrew
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
