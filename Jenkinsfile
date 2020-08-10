node {

    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'dockerHub') {

        def customImage = docker.build("hagenid/testpush")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
