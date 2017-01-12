#!/usr/bin/env groovy

node {
  stage('stage') {
    echo 'hello'

    echo currentBuild.changeSets.class.name
    for (ArrayList changetSet : currentBuild.changeSets) {
      echo changetSet.class.name
      echo changetSet.size.toString()
      for (entry in changetSet) {
        echo entry.class.name
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