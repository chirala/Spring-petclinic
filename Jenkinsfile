node('MVN') {
 stage('GIT') {
 git branch: 'Dev', url: 'https://github.com/chirala/spring-petclinic.git'
}
 stage('Build') {
    sh 'mvn package'
}
 stage('Archieve'){
 archive 'target//*.jar'
 junit 'target/surefire-reports/*.xml'
 }
}