# JenkinsSlaveSetup
Jenkins Slave Setup for windows

Required softwares to be installed on Master node

Java
Jenkins

Required softwares to be installed on Master node
Java (JRE)

create the nodes on the master node.

get the required files from the master node in the slave node.

http://jenkins-master:port/jnlpJars/slave.jar

http://jenkins-master:port/computer/node-name/slave-agent.jnlp  --> update node-name with machine name

http://jenkins-master:port/jnlpJars/agent.jar

clone the repo on slave node and update the jenkins-slave.xml accordingly.

to get the secret code open slave-agent.jnlp in notepad and copy the 64 bit hexa code available in application-desc main-class first argument.

make sure that you have all five files in one folder and open command prompt as administrator run below command

jenkins-slave.exe install --> to install as service.

jenkins-slave.exe start --> to start the service.

jenkins-slave.exe stop --> to stop the service.

jenkins-slave.exe uninstall --> to uninstall the service.

References

code for jenkins-slave.exe available at https://github.com/winsw/winsw

