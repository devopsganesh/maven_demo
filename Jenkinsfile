pipeline {
    agent any
    stages {
        stage ('SCM'){
            steps {git 'https://github.com/devopsganesh/maven_demo.git'}
        }
        stage ('BUILD'){
            steps {
                bat 'mvn clean'
                bat 'mvn install'
            }
        }
        stage ('DEPLOY'){
            steps {sh 'cp -r "C:\\Program Files\\Jenkins\\workspace\\modi\\gameoflife-web\\target\\gameoflife.war" "C:\\Program Files\\Apache Software Foundation\\Tomcat 8.5\\webapps\\test.war"'
                
            }
        }
    }
}
