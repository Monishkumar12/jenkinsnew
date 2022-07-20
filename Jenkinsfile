pipeline{
    agent any
    stages {
  stage('build') {
    steps {
      echo 'building';
    }
  }

  stage('test') {
    steps {
     echo 'testing';
    }
  }

  stage('deploy') {
    steps {
      echo 'deployed';
    }
  }
        steps {
        withMaven(globalMavenSettingsConfig: 'null', jdk: 'null', maven: 'null', mavenSettingsConfig: 'null') {
    sh 'mvn clean install'
}
        }
}


}
