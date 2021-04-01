Usage steps for Ubuntu 16.04:

Downloads
1. Download this repository
2. Download the folder "annotations" from 
3. Place the folder "annotations" in "data" folder
4. Download the file "model_50000" from
5. Place the file "model_50000" in "result" folder

Ubuntu setup
1. sudo apt-get update
2. sudo apt-get install build-essential checkinstall
3. sudo apt-get install -y build-essential tk-dev libncurses5-dev libncursesw5-dev libreadline6-dev libdb5.3-dev libgdbm-dev libsqlite3-dev libssl-dev libbz2-dev libexpat1-dev liblzma-dev zlib1g-dev libffi-dev tar wget vim
4. cd /opt
5. sudo wget https://www.python.org/ftp/python/3.8.5/Python-3.8.5.tgz
6. sudo tar xzf Python-3.8.5.tgz
7. cd Python-3.8.5
8. sudo ./configure --enable-optimizations
9. sudo make -j 4
10. sudo make altinstall
11. cd /opt
12. sudo rm -f Python-3.8.5.tgz
13. Change Directory to captionfyp_aavan
14. python3.8 -m pip install virtualenv
15. virtualenv -p python3.8 venv
16. source venv/bin/activate
17. pip install pandas
18. pip install dicttoxml
19. pip install opencv-python
20. pip install click
21. pip install Pillow
22. pip install chainer
23. sudo -i
24. echo 1 > /proc/sys/vm/overcommit_memory
