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
     echo "deploy" 
 }
}
}
}
