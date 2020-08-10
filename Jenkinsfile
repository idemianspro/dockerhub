node {

    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'testpush') {

        def customImage = docker.build("hagenid/testpush")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
