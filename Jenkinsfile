node {
    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'Docker_Hub_Credentials') {

        def customImage = docker.build("imyacoob86/docker-web-app:${env.BUILD_ID}")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}