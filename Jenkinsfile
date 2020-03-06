pipeline{
	agent any
	stages{
		stage('Clone'){
			steps{
			dir("D:\\CloneDIR\\version_$BUILD_ID") {
    			git branch: 'master', credentialsId: '3d5cdb37-6e90-465b-9b1d-527ae99e152d', url: 'https://github.com/Ritik180/Phase1-WithoutUsingBranches-.git'
				}
				echo "$BUILD_ID"
			}
			stage('Bootstrap Target Configuration'){
				steps{
					echo 'Bootstrap Done'
				}
			stage('Set Version'){
				steps{
					echo 'Set Version Done'
				}
			stage('MUnit Test'){
				steps{
					echo 'MUnit Test Done'
				}
			stage('Maven Build and Deploy to Exchange'){
				steps{
					echo 'Maven Build and Deploy to Exchange Done'
				}
			
			}
				
		}
	}
}
