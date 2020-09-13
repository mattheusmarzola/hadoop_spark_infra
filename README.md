# bd-infra
A development big data infrastructure with docker-compose.
<br> In this platform, you will have  HDFS, Hive, Spark, Hue, Zeppelin, Kafka, Zookeeper, and Streamsets connected together.
<br> Just run `docker-compose up` and enjoy!

<br> You can find more explenation in [this article](https://itnext.io/creating-a-big-data-development-platform-using-docker-compose-892f7f4da738).

Necessario criar uma rede externa e atribuir ao compose por problemas com o `_` no nome do dominio

* docker network create hadoopenv --subnet=172.27.0.0/16

No ambiente de desenvolvimento deve ser utilizado o python 3.7 e o spark 2.4.5 (pode ser utilizado criando um novo env no anaconda, ou pipenv)

* pip install pyspark==2.4.5

Caso esteja utilizando o anaconda e o JupyterLab, para o JupyterLab enxergar o novo env, deve ser utilizado os comandos abaixo:

* conda install ipykernel
* ipython kernel install --user --name=spark
