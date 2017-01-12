#!/usr/bin/env groovy

node {
  stage('stage') {
    echo 'hello'

    echo "ArrayList: ${currentBuild.changeSets.class.name}"
    for (ArrayList set : currentBuild.changeSets) {
      echo "GitChangeSetList: ${changetSet.class.name}"
      for (hudson.plugins.git.GitChangeSetList changeSetList in changetSet) {
        echo "GitChangeSet: ${changeSetList.class.name}"
        for (hudson.plugins.git.GitChangeSet changeSet in changeSetList) {
          echo changeSet.commitId
        }
      }
    }

    //         for ( in currentBuild.changeSets) {
                
    //                 for (file in entry.affectedFiles) {
    //                     echo "  ${file.editType.name} ${file.path}"
    // }

    // currentBuild.changeSets.each { changeset ->
    //   echo changeset
    //   echo changeset.class
    //   changeset.class.declaredFields.findAll { !it.synthetic }*.name.each { field ->
    //     echo field
    //   } 
    // }
  }
}