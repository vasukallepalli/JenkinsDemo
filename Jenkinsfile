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
          input ('Do you want to proceed?')

          echo ('This is Second step in pipeline')
       }
     }
     stage ('Three') {
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
