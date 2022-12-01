pipeline {
    agent any
    environment{
        PATH = "/opt/apache-maven-3.6.3/bin:$PATH"
    }
    stages {
        stage('Hello') {
            steps {
                git credentialsId: '122b4bed-9a7a-42c2-82ba-bbca62094dcd', url: 'https://github.com/PravinBalaji/hello-world.git'
            }
        }
        stage('Maven Build') {
            steps{
                sh "mvn clean package"
            }
        }
    }   
}
