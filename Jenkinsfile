pipeline {
    agent any

    stages {
        stage('Make_directory') {
            steps {
                echo 'I am creating new directory'
                deleteDir()
                bat 'mkdir mobeen'
            }
        }
        stage('inside_directory') {
            steps {
                echo 'I am inside direcoty'
                dir('C:\\ProgramData\\Jenkins\\.jenkins\\workspace\\basic_test_pipeline\\mobeen') {
                bat 'echo "hello" >> file.txt'
                }
                
                
            }
        }
        stage('create_file') {
            steps {
                echo 'I am creating new file'
                bat 'echo "hello" >> file.txt'
            }
        }
    }
}
