node {
    checkout scm

    docker.withServer('tcp://ec2-35-173-191-252.compute-1.amazonaws.com:2376', 'swarm-certs') {
        docker.image('mysql:5').withRun('-p 3306:3306') {
            /* do things */
        }
    }
}