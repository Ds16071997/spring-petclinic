node('openjdk11') {
stage('vcs') {
   git branch: 'sudhakar', url: 'https://github.com/Ds16071997/spring-petclinic.git'
}
stage('build') {
    sh '/usr/share/maven/bin/mvn package'
}
stage("archive results") {
    junit '**/surefire-reports/*.xml'
}
}
