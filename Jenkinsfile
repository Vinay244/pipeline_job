pipeline{
      
    agent any
    stages{
        stage('Hello_world'){
            steps
            {
                echo 'hello world'
                echo 'welcome to calsoft'
            }
        }
        stage('build'){
            steps
            {
                echo 'build done'
            }
        }
        stage('deploy'){
            steps
            {
                echo 'deploy done'
            }
        }
        stage('test'){
            steps
            {
                echo 'testing done'
            }
        }
        stage('vinay'){
              steps
              {
                    echo 'hiiii'
              }
        }
        stage('intern'){
              steps
              {
                  echo 'interns'  
              }
        
        }
        stage('check'){
             steps
            {
                echo 'check done'
                error "failed"
            }
        }
    }
    
    post
    {
        failure 
        {
            slackSend message:"Build failed  - ${env.JOB_NAME} ${env.BUILD_NUMBER} (<${env.BUILD_URL}|Open>)"
        }
        success {
            slackSend "Build deployed successfully - ${env.JOB_NAME} ${env.BUILD_NUMBER} (<${env.BUILD_URL}|Open>)"
        }
    }
}       
        
              
        
                  
    
