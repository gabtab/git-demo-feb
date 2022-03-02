pipeline{

    agent{ node{label 'master' } }
    parameters{
        string(name: 'FileName', defaultValue: '', description: 'Pls supply filename')
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
}
