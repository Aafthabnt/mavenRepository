pipeline{
	agent any
	tools{
	maven 
        
	} 
	stages{
	stage('checkout'){
	steps{
	git 'https://github.com/Aafthabnt/mavenRepository.git'
	}
   }
   stage('Build'){
   steps{
    sh 'mvn clean compile'
 }
}
stage('Test'){
steps{
sh 'mvn test'

}
}
stage('Package'){
steps{
	sh 'mvn package'
	}
	}
}
}
	