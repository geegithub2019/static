pipeline {
     agent any
     stages {
        stage('Upload to AWS') {
            steps {
              withAWS(region:'us-west-2',credentials:'Jenkins') {
                s3Upload(pathStyleAccessEnabled:true, payloadSigningEnabled: true, file:'index.html', bucket:'jenkese2019')
         }
        }
     }
  }
}
