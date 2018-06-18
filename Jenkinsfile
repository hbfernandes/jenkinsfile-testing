pipeline{
  agent {
    label 'non-master'  
  }
  stages {
    stage('Configure Pipeline') {
      steps {
        println 'configuration done'
      }
    }
    stage('Sequential Stage') {
      parallel {
        stage('Branch A') {
            steps {
                echo "On Branch A"
            }
        }
        stage('Branch B') {
            steps {
                echo "On Branch B"
            }
        }
      }
    }
  }
}
    