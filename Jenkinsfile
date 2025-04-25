node {
    stage('Clone Repository') {
        git branch: 'main', url : 'https://github.com/Rohit-Patil-24/s3-web-pp.git'
    }
    
    stage('Upload to S3') {
          sh '''
          aws s3 cp . s3://s3-pipeline-web-static/ --recursive
          '''
       }
  } 
