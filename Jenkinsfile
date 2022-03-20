pipeline{
	agent any
	tools{
	maven 'Maven 3.3.9' 
        jdk 'jdk8' 
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
	