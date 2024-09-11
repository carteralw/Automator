
library 'pipeline-library@main'
node {
    /* ... snip */
    withEnv(['NAME=Al']) {
        echo "My name is ${NAME}"
    }

    stage('lib call'){
        hello(name:"Al", dayOfWeek:"Wednesday")
    }
}