pipeline {
    agent any
    stages {
stage('scm') {
steps {
    git 'https://github.com/subrata171/maven_demo.git'
    }
}
    stage('build') {
    steps {
        echo "mvn clean install"
    }
}
    stage('junit') {
steps {
      echo "junit healthScaleFactor: 10.0, testResults: '**/gameoflife-web/target/surefire-reports/*.xml"
    }
}
    stage('deploy') {
steps {
     echo "bat 'copy "C:\\Program Files (x86)\\Jenkins\\workspace\\raghuproject\\gameoflife-web\\target\\*.war" "C:\\Program Files\\Apache Software Foundation\\Tomcat 9.0\\webapps\\" 
 }
}
}
}
