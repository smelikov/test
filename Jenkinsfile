node {
    stage('Preparation') { // for display purposes
      // Get some code from a GitHub repository
      git 'https://github.com/smelikov/test.git'
      
        
    }
   stage('Deploy_local') {
      // Run deploy
        checkout scm
        sh 'sudo pwd'
        sh 'sudo mv ./index.html /builds/index.html'
      } 
       
    stage('Upload_to_websrv') {
      
  }
   }
   stage('Results') {
      echo "URA!"
   }
