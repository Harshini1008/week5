
   pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                script {
                    echo 'Building Docker image...'
                    // Build the Docker image
                    sh 'docker build -t my-nodejs-appp-csed .'
                    // Replace this with actual Docker build command if needed
                    // sh 'docker build -t my-nodejs-appp-csed .'
                }
            }
        }
        stage('Test') {
            steps {
                script {
                    echo 'Running tests...'
                    // Add actual test commands if required
                    // For example, uncomment below if tests exist
                    // sh 'npm install'
                    // Replace this with actual test commands if needed
                    // sh 'npm test'
                }
            }
@@ -26,19 +23,8 @@ pipeline {
            steps {
                script {
                    echo 'Deploying application...'
                    // Run the application using Docker
                    sh 'docker run -d -p 8080:3000 my-nodejs-appp-csed'
                }
            }
        }
  stage('Release') {
            steps {
                script {
                    echo 'Releasing application...'
                    // Push Docker image to a registry if needed
                    // Uncomment and modify for release
                    // sh 'docker tag my-nodejs-appp-csed <your-dockerhub-username>/my-nodejs-appp-csed:latest'
                    // sh 'docker push <your-dockerhub-username>/my-nodejs-appp-csed:latest'
                    // Replace this with actual Docker run command if needed
                    // sh 'docker run -d -p 8080:3000 my-nodejs-appp-csed'
                }
            }
        }
