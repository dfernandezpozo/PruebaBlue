pipeline {
  agent any
  stages {
    stage('Inicio') {
      steps {
        echo 'INICIO'
        bat 'echo Empezando Pipeline'
      }
    }

    stage('Sistema') {
      steps {
        echo 'SISTEMA'
        bat 'echo %DATE% %TIME%'
      }
    }

    stage('Aprobacion') {
      steps {
        input(message: '¿Continuar a FIN?', ok: 'Continuar', cancel: 'NO')
      }
    }

    stage('Fin') {
      steps {
        echo 'FIN'
        echo 'FIN: empezando FIN: fecha y hora -> %DATE% %TIME% FIN: terminado'
      }
    }

  }
}