node {
    checkout scm

    environment { 
    HTTP_PROXY = 'http://forwardproxy.extnp.national.com.au:3128',
        HTTPS_PROXY = 'https://forwardproxy.extnp.national.com.au:3128'
}
    docker.withServer('tcp://10.39.152.14:2375', 'swarm-certs') {
        docker.image('mysql:5').withRun('-p 3306:3306') {
            /* do things */
        }
    }
}
