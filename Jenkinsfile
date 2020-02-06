node {
    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'dockerhubcred') {

        def customImage = docker.build("niteshsinghal88/nodejsapp")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
