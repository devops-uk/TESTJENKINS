pipeline {
  agent any
   stages {
   stage('build'){
   steps{
      sh 'docker build -f my-image/Dockerfile .'
   }
   }
      stage('Test') {
              steps {
                 
                     sh 'docker run -it Dockerfile'
                    echo "docker image tested"
                    }
           }
          stage('Deploy') {
              steps {
              sh 'docker run -it  Dockerfile'
                    sh 'docker push naveenkumaraluthuri Dockerfile'
                  }
            }
  }
 }
