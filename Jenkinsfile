pipeline {
  agent any
  stages {
    stage('prueba') {
      steps {
        parallel(
          "prueba": {
            echo 'hola mundo'
            
          },
          "uno paralelo": {
            sleep 10
            
          }
        )
      }
    }
    stage('paso3') {
      steps {
        catchError()
      }
    }
  }
}