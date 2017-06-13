pipeline {
  agent {
    node {
      label 'soa12clab'
    }
    
  }
  stages {
    stage('PreBuild Action') {
      steps {
        echo 'Initiating the Build Process'
      }
    }
    stage('CompileToWAR') {
      steps {
        sh '/opt/oracle/middleware/oracle_common/modules/org.apache.maven_3.2.5/bin/mvn package'
      }
    }
  }
}