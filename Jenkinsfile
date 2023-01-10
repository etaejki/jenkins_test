node {
    def hello = 'Hello Jenkins' 
    stage('Clone') {      
		steps {
			echo 'Clone'
			git branch: 'main', credentialsId: 'ktjt3', url: 'https://github.com/etaejki/jenkins_test.git' 
		}
    }

	stage ('execute') {
		sh './execute.sh'
	}
	
    stage ('print') {
        print(hello) 
    }
}

void print(message) {
    echo "${message}"
}
