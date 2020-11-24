# conda 

```bash
conda --version
conda update conda
conda --help
conda -h
rm -rf ~/anaconda3
conda create --name <env_name> <package_names>
e.g.:conda create -n python3 python=3.5 numpy pandas
source activate <env_name>
source deactivate
conda info --envs / conda info -e / conda env list
conda create --name <new_env_name> --clone <copied_env_name>
conda remove --name <env_name> --all
conda search --ful-name <package_full_name>
conda search <text>
conda list
conda install --name <env_name> <package_name>
conda install <package_name>
pip install <package_name>    (need to switch to env we want)
conda remove --name <env_name> <package_name>
conda remove <package_name>
conda update --all / conda upgrade --all
conda update <package_name> / conda upgrade <package_name>


```

