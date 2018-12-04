pipeline {
        agent none
        stage ('Clone') {
        git url: 'https://github.com/arunimmadi/sonar-scanner-jenkins'
    }
        stage ('Exec Maven') {
        rtMaven.run pom: 'sonar-scanner-jenkins/pom.xml', goals: 'clean install', buildInfo: buildInfo
    }   
      }


