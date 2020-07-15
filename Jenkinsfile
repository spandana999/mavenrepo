pipeline{
agent {label 'devserver'}
stages{
stage(scm){
steps{checkout([$class: 'GitSCM', branches: [[name: '*/feat01'], [name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'dfe6c534-1b8e-4466-9c75-cd0cbaca3950', url: 'https://github.com/spandana999/mavenrepo.git']]])
}
}
stage(mvn){
steps{
sh 'mvn package'
}

}

}
}
