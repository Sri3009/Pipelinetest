pipeline {
    agent any
    stages {
         stage('checkout'){
         steps{
         sh 'git checkout newtestbranch1'
         }
         }
         stage('create file'){
         steps{
         writeFile file: "newfile.txt", text: "This file is useful, need to archive it." 
         sh 'ls'
         sh 'cat newfile.txt'
         }
         }
         stage('add file'){
         steps{
         sh 'git add newfile2.txt'
         }
         }
        stage('commit changes'){
         steps{
         sh 'git commit -m "this is to test pipeline project from jenkins dashboard" newfile.txt'
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
