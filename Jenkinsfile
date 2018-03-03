node {
    stage('Preparation') { // for display purposes
      // Get some code from a GitHub repository
      git 'https://github.com/smelikov/test.git'
      
        
    }
   stage('Deploy') {
      // Run deploy
        checkout scm
        sh 'sudo pwd'
        sh 'sudo mv ./index.html /var/www/html/index.html'
      } 
   }
   stage('Results') {
      echo "URA!"
   }
