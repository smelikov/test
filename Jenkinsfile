node {
    stage('Preparation') { // for display purposes
      // Get some code from a GitHub repository
      git 'https://github.com/smelikov/test.git'
      
        
    }
   stage('Deploy_local') {
      // Run deploy
        checkout scm
        sh 'sudo pwd'
        sh 'sudo mv ./index.html /var/www/html/index.html'
      } 
    stage('Upload_to_websrv') {
      job('example') {
      steps {
         publishOverSsh {
            server('172.31.45.233') {
                transferSet {
                    sourceFiles('index.html')
                }
            }
        }
    }
  }
   }
   stage('Results') {
      echo "URA!"
   }
