---
layout: default
---

## Environment Setup

### APACHE Zeppelin
#### Description
Apache Zeppelin is a web-based notebook that enables interactive data analytics. You can think of it as a smart notepad++ with capabilities of reading and breaking down log files, analyzing the data using simple SQL like queries and displaying the results in a chart. It can be used as a reporting or dashboard module depending on your needs.

The tool can also be integrated with machine learning based tools for deep analytics and automation.

#### Installation
1. [All interpreterse](https://downloads.apache.org/zeppelin/zeppelin-0.9.0-preview1/zeppelin-0.9.0-preview1-bin-all.tgz):  Download the full Zeppelin Installer with all interpreters. (1.5 GB)
2. [Net-install interpreter package](https://downloads.apache.org/zeppelin/zeppelin-0.9.0-preview1/zeppelin-0.9.0-preview1-bin-netinst.tgz): Unpack the default setup and follow install additional interpreters to install interpreters. (723 MB)
  - Script to install all interpreters
    ```
    $   ./bin/install-interpreter.sh --all
    ```
  - Script to install specific interpreters
    ```
    $   ./bin/install-interpreter.sh --name md,jdbc,shell,python
    ```
  - Script to list interpreters
    ```
    $   ./bin/install-interpreter.sh --list
    ```

#### Requirements
- Java: Oracle JDK 1.7 and Above
- Operating System: Windows, Ubuntu, CentOS and macOS
- Python: Download the most recent and stable version of Python 2.7 and Python 3
  - Make sure you add python to your System environment variables before you try and run the command ‘python’ on your command-line.
  - [PIP](https://bootstrap.pypa.io/get-pip.py): Download the script from this link:  and run it on your command line as illustrated below:
    ```
    $  python  get-pip.py
    ```
- Machine Learning Libraries: Install this libraries using pip: Numpy, Scipy, Scikit-learn, Theano, TensorFlow, Keras, PyTorch, Pandas, Matplotlib
  ```
  $    pip install sklearn scikit-learn pyspark pandas numpy matploitlib scipy tensorflow keras pytorch
  $    pip3 install sklearn scikit-learn pyspark pandas numpy matploitlib scipy tensorflow keras pytorch
  ```
- Databases (Optional): Elasticsearch, MySQL, Oracle, PostgreSQL etc.
- Machine Learning Applications (Optional): Apache SPARK, Apache Hadoop, Apache Kafka etc.
- GIT: Optional for [Windows](https://git-scm.com/downloads) if you want a Linux based command line. 

#### Setup
- Start Apache Zeppelin by running the following commands:
  - On Unix like platforms
    ```
    $    bin/zeppelin-daemon.sh start
    ```
    ```
    $    bin/zeppelin-daemon.sh stop
    ```    
  - On Windows
    ```
    $    bin/zeppelin-daemon.cmd
    ```
    Wait until you see “Done, zeppelin server started” and go to your browser and access http://localhost:8080 

#### References
- https://zeppelin.apache.org/docs/latest/usage/interpreter/installation.html 
- https://zeppelin.apache.org/docs/latest/quickstart/install.html 

