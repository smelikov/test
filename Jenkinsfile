node {
    stage('Preparation') { // for display purposes
      // Get some code from a GitHub repository
      git 'https://github.com/smelikov/test.git'
      
        
    }
   stage('Deploy_local') {
      // Run deploy
        checkout scm
        sh 'sudo cp ./index.html /var/www/html/index.html'
   } 
       
    stage('Upload_to_websrv') {
        sh 'sudo cp ./index.html ../upload_ssh/index.html'
        build job: 'upload_ssh'    
  }
   }
   stage('Results') {
      echo "URA!"
   }
