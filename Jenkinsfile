pipeline {
   agent any
   stages {
     stages ('Build') {
       steps {
         echo 'Running Build Automation'
         sh './gradlew build --no daemon'
         archiveArtifacts artifacts: 'dist/trainschedule.zip'
       }
     }
   }
}
