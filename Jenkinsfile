pipeline{
	agent any
	tools{
	maven 'M3'
        
	} 
	stages{
	stage('checkout'){
	steps{
	git 'https://github.com/Aafthabnt/mavenRepository.git'
	}
   }
   stage('Build'){
   steps{
    bat 'mvn clean compile'
 }
}
stage('Test'){
steps{
bat 'mvn test'

}
}
//stage('Package'){
//steps{
//	sh 'mvn package'
	//}
	//}
}
}
	