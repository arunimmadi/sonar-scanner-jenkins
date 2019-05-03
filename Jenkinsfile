	pipeline {
        agent none
        stages {
          stage("edited the code") {
            agent any
            steps {
                bat 'mvn clean package sonar:sonar'
              }
            }
        }
      }
