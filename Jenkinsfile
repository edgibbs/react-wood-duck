node {
  stage "Prepare environment"
    checkout scm
    docker.image('node').inside {
      stage "Checkout and build deps"
        sh "yarn install"

        stage "Test and validate"
        sh "yarn test"
    }
}
