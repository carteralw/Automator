
library 'pipeline-library@main'
node {
    /* ... snip */
    withEnv(['NAME=Al']) {
        echo "My name is ${NAME}"
    }

    /*stage('lib call'){
        helloWorld(name:"Al", dayOfWeek:"Wednesday")
    }*/
    stage('brancher'){
        brancher('main'){
            sh -lsa
        }()
    }

    stage('hi'){
        helloWorld(name:"Al", dayOfWeek:"Wednesday")
    }

    stage('parallelling'){
        paralleler([
            'unit tests':{echo 'unit testing'},
            'integration tests':{echo 'integration testing'},
            'linting':{echo 'linting'},
        ])
    }
    
    stage('clock'){
        timer('build'){
            echo 'emitting information'
        }()
    }
}