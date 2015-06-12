# Storm Example for Twitter

This is a simple example of [Storm](https://storm.apache.org/) using the [Twitter4J](http://twitter4j.org/en/index.html)  to get the "Top N Hashtags" at the moment.
This code is based on the course [Real-Time Analytics with Apache Storm](https://www.udacity.com/course/real-time-analytics-with-apache-storm--ud381) from Udacity.

## Install

If you want to try out this code, follow these steps:

1. You need to install the following applications:
    1. [VirtualBox](https://www.virtualbox.org/)
    2. [Vagrant](https://www.vagrantup.com/)
2. Clone the project to your machine
3. Vagrant setup:
    1. Open a new console
    2. At the root folder type "vagrant up", this will create the virtual machine to run the solution
    3. At the root folder type "vagrant ssh" to connect to the VM
4. Build and running the Storm topology:
    1. Go into "/topology-topNHashTags"
    2. Type "mvn package" to compile the jar, this might take a while
    3. Type "storm jar target/storm.topology.topN-0.0.1-jar-with-dependencies.jar test.storm.TweetTopology"
6. Run the visualization page:
    1. Open a new console
    2. Go to "/viz"
    3. Type "python app.py"
    4. In your local machine open a browser a go to http://127.0.0.1:5000

## TODO
* Unit Testing