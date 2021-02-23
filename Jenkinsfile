pipeline {
  agent any
    
  tools {nodejs "Nodejs 4.8.6"}
    
  stages {
        
    stage('Cloning Git') {
      steps {
        git 'https://github.com/sarathchandrankp/front-end.git'
      }
    }
        
    stage('Install dependencies') {
      steps {
        sh 'npm install'
      }
    }
     
    stage('Test') {
      steps {
         sh 'npm test'
      }
    }
	stage('Package') {
	  steps  {
		sh 'npm run package'
	  }
	}
	
  }
 
}
