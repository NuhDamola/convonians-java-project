pipeline {
    agent any

    stages {
        stage('Test') {
            steps {
                sh 'cd SampleWebApp && mvn test'
            }
        }
        stage('Build') {
            steps {
                sh 'cd SampleWebApp && mvn clean package'
            }
        }
        //  stage('Deploy to Tomcat') {
        //     steps {
        //         deploy adapters: [tomcat9(credentialsId: 'tomocatpassowrd', path: '', url: 'http://54.173.162.186:8080/')], contextPath: 'myapp', war: '**/*.war'
        //     }
        // }
  
    }
}
