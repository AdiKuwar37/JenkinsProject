node('master') {
   stage('Build') {
     echo 'Building...'
   }
   stage('Test') {
      echo 'Testing..'
   }
   stage('Deploy') {
     sshagent (credentials: ['9fbaa4de-9744-4954-81a6-c82711349737']) {
        sh 'ssh -o StrictHostKeyChecking=no -T https://github.com'
        sh "git clone https://github.com/AdiKuwar37/npmjs-publish.git"
     }
   }
}
