# python-resources
Assignment 1
Spark Environment
Hardware configuration: One m5.2xlarge master node, Three m5.2xlarge core nodes
Software configuration: EMR release 5.29, Spark 2.4.4, TensorFlow 1.14.0, Livy 0.6.0, Hadoop 2.8.5
Bootstrap files are in the Assignment 1 folder 

Add the following into Enter configuration in the software configuration steps
[{"classification":"spark","properties":{"maximizeResourceAllocation":"true"}},{"classification":"livy-conf","properties":{"livy.server.session.timeout-check":"true","livy.server.session.timeout":"3h","livy.server.yarn.app-lookup-timeout":"120s"}}]
