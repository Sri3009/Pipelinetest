pipeline {
    agent any
    stages {
         stage('checkout'){
         steps{
         sh 'git checkout newtestbranch'
         }
         }
         stage('create file'){
         steps{
         writeFile file: "newfile1.txt", text: "This file is useful, need to archive it." 
         sh 'ls'
         sh 'cat newfile1.txt'
         }
         }
         stage('add file'){
         steps{
         sh 'git add newfile1.txt'
         }
         }
        stage('commit changes'){
         steps{
         sh 'git commit -m "this is to test pipeline project from jenkins dashboard" newfile1.txt'
         }
         }
    stage('push'){
         steps{
         sh 'git push origin newtestbranch'
         }
         }

stage('message') {
            steps {
                sh 'echo "successfully finished"'
         
                
            }
        }
    }
}
