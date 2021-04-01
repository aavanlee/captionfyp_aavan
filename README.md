Usage steps for Ubuntu 16.04:

Downloads
1. Download/clone this repository
2. Download the folder "annotations" from https://www.dropbox.com/sh/fg1timcbrcdyhye/AAAs6z-ggS02ZFsVKhSLIUEEa?dl=0
3. Place the folder "annotations" in "data" folder
4. Download the file "model_50000" from https://www.dropbox.com/s/4rq62ru3ec9wdjk/model_50000?dl=0
5. Place the file "model_50000" in "result" folder

Ubuntu python setup
1. sudo apt-get update
2. sudo apt-get install build-essential checkinstall OR sudo apt --fix-broken install FIRST
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

Ubuntu setup
14. Change Directory to captionfyp_aavan
15. python3.8 -m pip install virtualenv
16. virtualenv -p python3.8 venv
17. source venv/bin/activate
18. pip install pandas
19. pip install dicttoxml
20. pip install opencv-python
21. pip install click
22. pip install Pillow
23. pip install chainer
24. sudo -i
25. echo 1 > /proc/sys/vm/overcommit_memory
26. cd cocoapi
27. cd PythonAPI
28. pip install -e.
29. cd ..
30. cd ..

Run
1. Put videos in "videos" folder, existing videos are: "airplane.mp4, bees.mp4, covid.mp4,"
2. Run from terminal using $ python full.py <video_name>
3. Example: python full.py airplane.mp4
