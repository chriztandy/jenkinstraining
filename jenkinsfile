pipeline {
    agent any

    stages {
        stage('Step One') {
            steps {
               bat 'dir c:\\windows > hasil.txt'
            }
        }
        stage('Step Two') {
            steps {
               bat 'copy hasil.txt c:\\latihan'
            }
        }
        stage('Step Three') {
            steps {
               bat 'del c:\\latihan\\result.txt'
               bat 'cd c:\\latihan'
               bat 'ren hasil.txt result.txt'
            }
        }
    }
}
