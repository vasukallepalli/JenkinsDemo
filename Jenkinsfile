pipeline {
  agent any
  stages {
     stage ('First') {
       steps {
         echo ('This is first step in pipeline')
       }
     }
     stage ('Second') {
       steps {
         echo ('Do you want to proceed?)
       }
     }
     stage ('Second') {
        when {
          not {
              branch "master"
          }
        }
       steps {
          echo ('This is Third step in pipeline')
       }
     }
  }

}
