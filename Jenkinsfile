pipeline {
    agent any
    stages {
        stage('Create branch'){
          steps{
            sh 'git branch newtestbranch2'
            }
           }
         stage('checkout'){
         steps{
         sh 'git checkout newtestbranch2'
         }
         }
         stage('create file'){
         steps{
         sh 'touch newfile'
         sh 'ls'
         }
         }
         stage('add file'){
         steps{
         sh 'git add .'
         }
         }
         stage('commit changes')
         steps{
         sh 'git commit -am "this is to test pipeline project from jenkins dashboard"'
         }
         }
    stage('push'){
         steps{
         sh 'git push origin newtestbranch2'
         }
         }

stage('message') {
            steps {
                sh 'echo "successfully finished"'
         
                
            }
        }
    }
}
