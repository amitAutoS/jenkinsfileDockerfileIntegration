node {
    checkout scm

    docker.withServer('tcp://0.0.0.0:2376', 'swarm-certs') {
        docker.image('mysql:5').withRun('-p 3306:3306') {
            /* do things */
        }
    }
}