pipeline{
    agent any
    stages{
        stage("git checkout"){
            steps{
                checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/hemanth625/maven-simple.git']]])
            }
        }
                stage("build"){
            steps{
                sh "echo build"
            }
        }
                stage("UPLOAD ARTIFACTORY"){
            steps{
                sh "echo upload"
            }
        }
                stage("deployment"){
            steps{
                sh "echo test"
            }
        }
                stage("testing"){
            steps{
                sh "echo test"
            }
        }
    }
}
