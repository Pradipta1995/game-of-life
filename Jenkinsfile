node('tester1') {
    
    stage('git') {
         git branch: 'Dev', url: 'https://github.com/Pradipta1995/game-of-life.git'
    }
    stage('build') {
    sh 'mvn package'
    }
}