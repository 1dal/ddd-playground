podTemplate(label: 'jnlp', containers: [
    containerTemplate(
          name: 'jnlp',
          image: 'eggsy84/gcp-jenkins-slave-k8s-seed:latest',
          ttyEnabled: false,
          command: '',
          privileged: true,
          alwaysPullImage: false,
          workingDir: '/home/jenkins',
          args: '${computer.jnlpmac} ${computer.name}'
        )
    ],
    volumes: [
          hostPathVolume(mountPath: '/var/run/docker.sock', hostPath: '/var/run/docker.sock')
    ]
)

{

  node('jnlp') {

      stage('Say hello') {
        echo "hola que ase"
      }
  }
}