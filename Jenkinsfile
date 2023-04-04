pipeline{
	agent any
	stages{
		stage('1-clone'){
			steps{
				checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'team5-id', url: 'https://github.com/Team5-group6/parralele-job.git']])
			}
		}
		stage('2-parralel-stage'){
			parralel{
				stage('1-parralel-saada-job'){
					steps{
						sh'lscpu'
					}
				}
				stage('2-parrale-aubin-job'){
					steps{
						sh 'du -h'
					}
				}
			}
		}
	}
}
