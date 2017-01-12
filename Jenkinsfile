#!/usr/bin/env groovy

def getCommitId() {
  for (ArrayList list : currentBuild.changeSets) {
    for (hudson.plugins.git.GitChangeSetList changeSetList in list) {
      for (hudson.plugins.git.GitChangeSet changeSet in changeSetList) {
        return changeSet.commitId
      }
    }
  }
  throw new RuntimeException("commitId unavailable")
}

node {
  stage('stage') {
    echo getCommitId()

    echo scm.class.name
  }
}