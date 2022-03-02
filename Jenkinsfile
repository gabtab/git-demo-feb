pipeline{

    agent{ node{label 'master' } }
    parameters{
        string(name: 'FileName', defaultValue: '', description: 'Pls supply filename')
        choice(name: 'FileList', choices:['demo.txt', 'gavin.txt'], description; 'Pick file for testing')
    }

    stages{
    stage('Read demo file'){
        steps{
             sh "cat ${params.FileName}"
        }
    }
    stage('Read Readme.md file'){
        steps{
             sh 'cat README.md'
        }
    }
      }
    stage('Read file from choice'){
        steps{
             sh "cat ${params.FileList}"
        }
    }
}
}
