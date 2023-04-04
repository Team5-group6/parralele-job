pipeline{
	agent any
	stages{
		stage('1-clone'){
			steps{
				'action1'
			}
		}
		stage('2-parralel-stage'){
			parralele{
				stage('1-parralel-saada-job'){
					steps{
						'action parralel-subjob1'
					}
				}
				stage('2-parrale-aubin-job'){
					steps{
						'action parralel-subjob2'
					}
				}
			}
		}
	}
}
