pipeline{

	agent any

	stages{
		stage('Clone'){
			steps{
			        dir("D:\\CloneDIR\\version_$BUILD_ID") {

    			git branch: 'master', credentialsId: '3d5cdb37-6e90-465b-9b1d-527ae99e152d', url: 'https://github.com/Ritik180/CI-CD Pipeline-.git'

				}

				echo "$BUILD_ID"

			}

		}

		stage('BootStrap with TargetConfiguration'){

			steps{

				configFileProvider([configFile(fileId: 'dev-sys', targetLocation: "D:\\CloneDIR\\version_$BUILD_ID", variable: 'dfvdf')]) {

    				// some block

    				echo "$dfvdf"

				}

			}

		}

	}

}
