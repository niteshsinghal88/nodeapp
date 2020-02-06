node {
    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'dockerhubcred') {

        def customImage = docker.build("app/nodejswebapp")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
