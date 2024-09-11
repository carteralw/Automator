
library 'pipeline-library@main'
node {
    /* ... snip */
    withEnv(['NAME=Al']) {
        echo "My name is ${NAME}"
    }

    stage('lib call'){
        helloWorld(name:"Al", dayOfWeek:"Wednesday")
    }
}