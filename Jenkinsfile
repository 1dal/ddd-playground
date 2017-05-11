podTemplate(label: 'ddd-ci', containers: [
        containerTemplate(name: 'jnlp', image: 'jenkinsci/jnlp-slave:2.62-alpine', args: '${computer.jnlpmac} ${computer.name}')
    ]) {
    node('ddd-ci') {
        stage('Run shell') {
            sh 'echo hello world'
        }
    }
}
