pipeline {
    agent any

    stages {
        stage('Build') {
            steps {

                                   
                    // Run Shell Script to Build Client Docker Image.
                    sh "sudo /home/aj/workspace/mean-stack/client/buildClient.sh"

                    // Run Shell Script to Build Server Docker Image.
                    sh "sudo /home/aj/workspace/mean-stack/server/buildServer.sh"
 
                

            }
        }
        
        stage('Deploy') {
            steps {
                
                    // Run Shell Script to Deploy Server.
                    sh "sudo /home/aj/workspace/mean-stack/deployServer.sh"
    
                    // Run Shell Script to Deploy Client.
                    sh "sudo /home/aj/workspace/mean-stack/deployClient.sh"
                }
            
        }

    }
}
