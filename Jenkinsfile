#!/usr/bin/env groovy

node {
  stage('stage') {
    echo 'hello'
    currentBuild.changeSets.each { changeset ->
      echo changeset
      echo changeset.class
      changeset.class.declaredFields.findAll { !it.synthetic }*.name.each { field ->
        echo field
      } 
    }
  }
}