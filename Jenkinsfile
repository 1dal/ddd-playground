podTemplate(label: 'ddd-ci', containers: [
        containerTemplate(name: 'jnlp', image: 'jenkinsci/jnlp-slave:2.62-alpine', args: '${computer.jnlpmac} ${computer.name}'),
        containerTemplate(name: 'debian', image: 'debian')
    ]) {
    node('ddd-ci') {
        stage('Run shell') {
            container("debian") {

                sh 'echo hello world'
            }
        }
    }
}
