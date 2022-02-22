node { 
  stage('========== Clone repository ==========') 
  { 
    checkout scm
  } 
  stage('========== Build image ==========') 
  { 
    app = docker.build("demo/demo") 
  } 
  stage('========== Push image ==========') 
  { 
    docker.withRegistry('yyouri', 'yyouri') {
    
    app.push("${env.BUILD_NUMBER}") app.push("latest")
    } 
  } 
}

