pipeline {
  agent {
    node {
      label 'master'
    }
    
  }
  stages {
    stage('PreBuild Action') {
      steps {
        echo 'Initiating the Build Process'
      }
    }
    stage('Setting Maven Path') {
      steps {
        bat 'set PATH=%PATH%;C:\\JDEV12R2V1SOA\\oracle_common\\modules\\org.apache.maven_3.2.5\\bin'
      }
    }
    stage('Creating Package') {
      steps {
        bat 'mvn package'
      }
    }
  }
}