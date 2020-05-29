pipeline {
  agent any
  stages {
    stage('Download code') {
      steps {
        git(url: 'git@github.com:robertoarcomano/Test-git.git', branch: 'master')
      }
    }

    stage('Execute command') {
      steps {
        sh 'ls -al '
      }
    }

    stage('Archive artifact') {
      steps {
        archiveArtifacts '*'
      }
    }

  }
}