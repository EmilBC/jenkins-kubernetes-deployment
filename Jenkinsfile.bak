node {
    def mvnHome = tool 'maven-3.9.2'
    def dockerImage
    def dockerImageTag = "devopsexample${env.BUILD_NUMBER}"
    
    stage('Clone Repo') {
      git 'https://github.com/EmilBC/branch.git'
      
    }

   
  
    stage('Build Project') {
      sh "'${mvnHome}/bin/mvn' -B -DskipTests clean package"
    }
    
    
}


