pipeline {
  agent any
  tools { 
        maven 'maven-3.6.2' 
        jdk 'jdk8' 
  }
  stages {
    stage ('Initialize') {
            steps {
                sh '''
                    echo "PATH = ${PATH}"
                    echo "M2_HOME = ${M2_HOME}"
                ''' 
       }
    }
    stage('install') {
      steps {
        sh 'mvn clean install'
      }
    }
  }
}
