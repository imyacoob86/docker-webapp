node {
    checkout scm

    docker.withRegistry('https://hub.docker.com', 'Docker_Hub') {

        def customImage = docker.build("imyacoob86/docker-webapp")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
