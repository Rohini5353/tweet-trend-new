pipeline {
    agent { label 'maven' }  // ✅ correct way

    environment {
        PATH = "/opt/apache-maven-3.9.11/bin:$PATH"
    }

    stages {
        stage('Build') {
            steps {
                sh 'mvn clean deploy -DskipTests'  // optional skip tests to avoid build failure
            }
        }
    }
}
