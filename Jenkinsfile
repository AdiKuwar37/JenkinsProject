node('master') {
   stage('Build') {
     echo 'Building...'
   }
   stage('Test') {
      echo 'Testing..'
   }
   stage('Deploy') {
     sshagent (credentials: ['cc22f551-f409-47f0-8f54-01478773b1a6']) {
        sh "git clone https://github.com/AdiKuwar37/npmjs-publish.git"
     }
   }
}
