node {

 stage 'Stage 1'
   echo 'We are about to pretend that some of our Jenkins run is machine specific'
   echo 'This allows us to keep our infrastucture as code clean'
   echo 'see 12factor for the basic idea of what to keep in environment variables'
   echo 'JAVA_HOME is printed to the screen below'
   echo 'If this had been a real project, you might use environment variables to configure a portion of your Jenkins run'
   echo 'that you did not want to commit to source because every Jenkins server should run it differently'
   echo 'notice that this fails to echo JAVA_HOME ${env.JAVA_HOME} due to single quotes'   
   echo "JAVA_HOME is ${env.JAVA_HOME} on this machine"   
}
/*
stage 'Print All Environmental Variables'
node {
    println 'Printing all the Environmental Variables'
    bat 'env > env.txt'
    readFile('env.txt').split("\r?\n").each {
        println it
    }
    println "Done printing all the Environmental Variables"
}
*/

node{
	stage "Printing Maven Env Variable"
	def mvnGene= tool 'M3'
	println mvnGene
	echo mvnGene
	def mvnHome = tool 'Maven 3.3.9' 
    println mvnHome
    echo "PATH= ${PATH}"
	echo "M2_HOME= ${M2_HOME}"
    echo "mvnHome= ${mvnHome}"
}
