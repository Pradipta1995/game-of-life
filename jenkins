node('tester1') {
    
    stage('git') {
         git branch: 'Dev', url: 'https://github.com/Pradipta1995/game-of-life.git'
    }
    stage('build') {
		 sh 'mvn package'
    }
	stage('Archive') {
		 archive 'gameoflife-web/target/*.war'
		 junit 'gameoflife-web/target/surefire-reports/*.xml'
	}
}