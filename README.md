# Data Engineering: Pipeline Implementation
# Case Study Description: 
The case study aims to create a Data Science Application and service an ETL pipeline for an employee scheduling system for a 24/7 operational environment deployed in a Kubernetes Cluster following the below restrictions and considerations.
  * No employee should be alone in their shift
  * Ensure that night shifts have at least two (2) or (3) members
  * A 24-hr shift operation is divided into 3 shifting schedules: Morning, Mid and Night shift
  * An employee should only go to work for 5 days per week
  * The shift of an employee changes once a month

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

### Link for the Full Documentation:
https://docs.google.com/document/d/1M6kPuR1pQQcd-McMTnXzjviUePms_e3lHSA03k9T4Mg/edit?usp=sharing

github repo used for the Airflow DAG files and pysparkjob for scheduling: https://github.com/opswerks/test-airflow-dags








