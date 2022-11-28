
 sudo apt-get install maven
 
 mvn --version
 
 tar -xvf openjdk-13.0.1_linux-x64_bin.tar.gz
 
 JAVA_HOME='/opt/jdk-13.0.1'
 
 PATH="$JAVA_HOME/bin:$PATH"
 
 export PATH
 
 java -version
 
 apt install default-jre
 
 sudo apt install default-jre
 
 sudo apt install openjdk-11-jre-headless
 
 sudo apt-get update --fix-missing
 
 sudo apt install openjdk-11-jre-headless
 
 java -version
 
 wget https://mirrors.estointernet.in/apache/maven/maven-3/3.6.3/binaries/apache-maven-3.6.3-bin.tar.gz
 
tar -xvf apache-maven-3.6.3-bin.tar.gz

mv apache-maven-3.6.3 /opt/

sudo mv apache-maven-3.6.3 /opt/

M2_HOME='/opt/apache-maven-3.6.3'

PATH="$M2_HOME/bin:$PATH"

export PATH

mvn --version
