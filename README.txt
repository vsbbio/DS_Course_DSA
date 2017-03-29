#Jupyter Notebook's from Data Science Academy running in Cloud9 VM 

##How to install 'Jupyter Notebook' in Cloud9

###Installing miniconda
bash wget "https://repo.continuum.io/miniconda/Miniconda3-latest-Linux-x86_64.sh"
bash chmod a+x Miniconda3-latest-Linux-x86_64.sh
bash ./Miniconda3-latest-Linux-x86_64.sh

###Installing Jupyter
bash conda install jupyter
bash jupyter notebook --ip=0.0.0.0 --port=8080 --no-browser

###Creating an alias to Jupyter
bash cd ~/
bash nano .bash_aliases

"" edit the file and write down:" 
bash alias jupyter='jupyter notebook --ip=0.0.0.0 --port=8080 --no-browser'

^X #to exit
Y #save the file
Enter #back terminal



