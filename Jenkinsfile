pipeline {
    agent any
    stages {
        stage('create branch')
        steps{
            sh 'git branch newtestbranch4'
        }
    }
         stage('checkout'){
         steps{
         sh 'git checkout newtestbranch4'
         }
         }
         stage('create file'){
         steps{
         writeFile file: "newfile2.txt", text: "This file is useful, need to archive it." 
         sh 'ls'
         sh 'cat newfile2.txt'
         }
         }
         stage('add file'){
         steps{
         sh 'git add newfile2.txt'
         }
         }
        stage('commit changes'){
         steps{
         sh 'git commit -m "this is to test pipeline project from jenkins dashboard" newfile2.txt'
         }
         }
    stage('push'){
         steps{
         sh 'git push origin newtestbranch4'
         }
         }

stage('message') {
            steps {
                sh 'echo "successfully finished"'
         
                
            }
        }
    }
}
