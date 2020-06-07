---
layout: default
---

## Environment Setup

### APACHE Zeppelin
#### Description
Apache Zeppelin is a web-based notebook that enables interactive data analytics. You can think of it as a smart notepad++ with capabilities of reading and breaking down log files, analyzing the data using simple SQL like queries and displaying the results in a chart. It can be used as a reporting or dashboard module depending on your needs.

The tool can also be integrated with machine learning based tools for deep analytics and automation.

#### Installation
1. All Interpreters:  Download the full Zeppelin Installer with all interpreters which include: 
    ◦ Link: https://downloads.apache.org/zeppelin/zeppelin-0.9.0-preview1/zeppelin-0.9.0-preview1-bin-all.tgz  (1.5 GB)
2. Net-install interpreter package: Unpack the default setup and follow install additional interpreters to install interpreters. 
    ◦ Link: https://downloads.apache.org/zeppelin/zeppelin-0.9.0-preview1/zeppelin-0.9.0-preview1-bin-netinst.tgz (723 MB)
    ◦ Script to install all interpreters

    ◦ Script to install specific interpreters

    ◦ Script to list interpreters


#### Requirements
 • Java: Oracle JDK 1.7 and Above
 • Operating System: Windows, Ubuntu, CentOS and macOS
 • Python: Download the most recent and stable version
    ◦ Python 2.7
       ▪ Windows:  https://www.python.org/ftp/python/2.7.18/python-2.7.18.amd64.msi 
    ◦ Python 3
        ▪ Windows: https://www.python.org/ftp/python/3.8.3/python-3.8.3-amd64.exe 

  Make sure you add python to your System environment variables before you try and run the command ‘python’ on your command-line.
    ◦ PIP: Download the script from this link: https://bootstrap.pypa.io/get-pip.py and run it on your command line as illustrated below:

    ◦ Machine Learning Libraries: Install this libraries using pip: Numpy, Scipy, Scikit-learn, Theano, TensorFlow, Keras, PyTorch, Pandas, Matplotlib
    • Databases (Optional): Elasticsearch, MySQL, Oracle, PostgreSQL etc.
    • Machine Learning Applications (Optional): Apache SPARK, Apache Hadoop, Apache Kafka etc.
    • GIT: Optional for Windows if you want a Linux based command line.
        ◦ Linux: https://git-scm.com/downloads 

#### Setup
    • Start Apache Zeppelin by running the following commands:
        ◦ On Unix like platforms


        ◦ On Windows

Wait until you see “Done, zeppelin server started” and go to your browser and access http://localhost:8080 

#### References
    • https://zeppelin.apache.org/docs/latest/usage/interpreter/installation.html 
    • https://zeppelin.apache.org/docs/latest/quickstart/install.html 

