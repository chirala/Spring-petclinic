node('MVN') {
 stage('GIT') {
 git branch: 'Dev', url: 'https://github.com/chirala/spring-petclinic.git'
}
 stage('Build') {
    sh 'mvn install'
}
 stage('dummy')
 {
 sh 'pwd'
 }
 stage('Archieve'){
 archive 'target//*.jar'
 junit 'target/surefire-reports/*.xml'
 }
}