# Coffee-Break-Enjoyer

Drop your resources here guys :)

>> WEB LINK -- In that folder you can drop video and resources links


## Setting up your local machine to connect to kubernetes cluster provided by the mentors
follow the installation process here:
https://kubernetes.io/docs/tasks/tools/install-kubectl-macos/

download a2t-pe-cs1-F-kubeconfig.yaml and store it to your home dir
```sh
mv ~/Downloads/a2t-pe-cs1-F-kubeconfig.yaml ~
```
```sh
export KUBECONFIG=~/a2t-pe-cs1-F-kubeconfig.yaml
```
try this command to confirm connection to the cluster:
```sh
kubectl cluster-info
```
```sh
kubectl config view
```
```sh
kubectl get nodes
```








## Setting up the pyspark environment
install brew on your mac 
```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```
```sh
brew --version
```
install python3, scala, openjdk@11, apache-spark and jupyter notebook
```sh
brew install python3
```
```sh
brew install scala
```
```sh
brew install openjdk@11
```
```sh
brew install apache-spark
```
```sh
brew install jupyterlab
```

To check if everything is installed successfully:
```sh
spark-submit --version
```
```sh
jupyter notebook
```
```sh
python3 --version
```







