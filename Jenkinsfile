node{
	stage "Printing Maven Env Variable"
	/*
	def workspace= pwd()
	println workspace

    def buildprops = readProperties file: './properties/build.properties'
    println buildprops
    
	echo 'workspace= WORKSPACE'
	print "MAVEN_HOME is ${env.MAVEN_HOME} on this machine"
    echo "javaHome= ${%JAVA_HOME%}"
    */
}

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

