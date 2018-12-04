pipeline {
        agent none
        stage ('Clone') {
        git url: 'https://github.com/arunimmadi/sonar-scanner-jenkins'
    }
        stage ('Exec Maven') {
        rtMaven.run pom: 'sonar-scanner-jenkins/pom.xml', goals: 'clean install', buildInfo: buildInfo
    }
        stages {
          stage("build & SonarQube analysis") {
            agent any
            steps {
              withSonarQubeEnv('My SonarQube Server') {
                sh 'mvn clean package sonar:sonar'
              }
            }
          }
      }
   }

