
node {
  stage('checkout sources') {
        // You should change this to be the appropriate thing
        git url: 'https://github.com/VidyaRajesh2019/completing-assignment-lab-CI', branch:'completing-assignment-lab-CI'
  }

  stage('Build') {
    // you should build this repo with a maven build step here
     withMaven (maven: 'maven3') {
              sh "mvn package"
            }
  }

   stage('Test') {
      // you should build this repo with a maven build step here
       withMaven (maven: 'maven3') {
                sh "mvn test"
              }
    }


}
