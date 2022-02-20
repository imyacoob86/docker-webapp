node {
    checkout scm

    docker.withRegistry('https://hub.docker.com', 'docker_hub') {

        def customImage = docker.build("imyacoob86:docker-webapp")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}