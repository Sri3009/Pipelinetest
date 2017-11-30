pipeline {
    agent any
    stages {
         stage('checkout'){
         steps{
         sh 'git checkout newtestbranch3'
         }
         }
         stage('create file'){
         steps{
   
         writeFile file: "newfile1.txt", text: "This file is useful, need to archive it." 
         sh 'ls'
         }
         }
         stage('add file'){
         steps{
         sh 'git add .'
         }
         }
        stage('commit changes'){
         steps{
         sh 'git commit -m "this is to test pipeline project from jenkins dashboard" newfile'
         }
         }
    stage('push'){
         steps{
         sh 'git push origin newtestbranch3'
         }
         }

stage('message') {
            steps {
                sh 'echo "successfully finished"'
         
                
            }
        }
    }
}
