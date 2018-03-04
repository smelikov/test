node {
    stage('Preparation') { // for display purposes
      // Get some code from a GitHub repository
      git 'https://github.com/smelikov/test.git'
      
        
    }
   stage('Deploy_local') {
      // Run deploy
        checkout scm
        sh 'sudo cp ./index.html ../upload_ssh/index.html'
        sh 'sudo pwd'
   } 
       
    stage('Upload_to_websrv') {
        
            steps {
                script {
                    build(job: "upload_ssh",
                                       
            }
        }
      
  }
   }
   stage('Results') {
      echo "URA!"
   }
