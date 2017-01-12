#!/usr/bin/env groovy

node {
  stage('stage') {
    echo 'hello'

    echo "ArrayList: ${currentBuild.changeSets.class.name}"
    for (ArrayList changetSet : currentBuild.changeSets) {
      echo "GitChangeSetList: ${changetSet.class.name}"
      for (hudson.plugins.git.GitChangeSetList changeSetList in changetSet) {
        echo "Unknown: ${changeSetList.class.name}"
        for (item in changeSetList) {
          echo item.class.name
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