node {
    stage('Preparation') { // for display purposes
      // Get some code from a GitHub repository
      git 'https://github.com/smelikov/test.git'
      
        
    }
   stage('Deploy') {
      // Run the maven build
        sh 'sudo pwd'
        sh 'sudo mv ./index /var/www/html/index.html'
      } 
   }
   stage('Results') {
      echo "URA!"
   }
