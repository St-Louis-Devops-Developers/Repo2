node
{
    stage('Checkout')
    {
        checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/bhargav570392/githubtest.git']]])
    }
     stage('mail')
    {
        step([$class: 'Mailer', notifyEveryUnstableBuild: true, recipients: 'brahminikatta@gmail.com', sendToIndividuals: false])
    }
}
