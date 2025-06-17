#!/usr/bin/env groovy

pipeline {
  agent any
    stages {
      stage('Build') {
        steps {
          checkout scm
          sh 'USER_UID=997 GROUP_UID=995 ./build.sh init clean install publish'
        }
      }
    }
}

