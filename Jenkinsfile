pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                echo 'Stage 1: Build'
                echo 'Task: Compiling and packaging the application source code.'
                echo 'Tool: Maven - compiles Java source files and packages them into a JAR/WAR artifact.'
            }
        }

        stage('Unit and Integration Tests') {
            steps {
                echo 'Stage 2: Unit and Integration Tests'
                echo 'Task: Running unit tests to verify individual functions, and integration tests to verify components work together.'
                echo 'Tools: JUnit for unit testing, Selenium for integration testing.'
            }
        }

        stage('Code Analysis') {
            steps {
                echo 'Stage 3: Code Analysis'
                echo 'Task: Analysing source code for style issues and adherence to coding standards.'
                echo 'Tool: Checkstyle via Jenkins plugin to enforce Java coding standards.'
            }
        }

        stage('Security Scan') {
            steps {
                echo 'Stage 4: Security Scan'
                echo 'Task: Scanning dependencies for known CVEs and vulnerabilities.'
                echo 'Tool: OWASP Dependency-Check to identify vulnerable libraries.'
            }
        }

        stage('Deploy to Staging') {
            steps {
                echo 'Stage 5: Deploy to Staging'
                echo 'Task: Deploying the packaged application to a staging server.'
                echo 'Tool: AWS CLI used to deploy to an AWS EC2 staging instance.'
            }
        }

        stage('Integration Tests on Staging') {
            steps {
                echo 'Stage 6: Integration Tests on Staging'
                echo 'Task: Running integration tests on staging to confirm production-like behaviour.'
                echo 'Tool: Selenium WebDriver for automated browser-based integration testing.'
            }
        }

        stage('Deploy to Production') {
            steps {
                echo 'Stage 7: Deploy to Production'
                echo 'Task: Deploying the verified application to the live production server.'
                echo 'Tool: AWS CLI used to deploy to an AWS EC2 production instance.'
            }
        }
    }
}
