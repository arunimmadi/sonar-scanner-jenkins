pipeline {
        agent none
        stages {
          stage("build & SonarQube analysis") {
            agent any
            steps {
                bat 'mvn clean package sonar:sonar'
              }
            }
        }
      }
