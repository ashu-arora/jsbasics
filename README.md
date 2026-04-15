# jsbasics
Java Script  Bignners
https://freelance-learn-automation.vercel.app/login


library identifier: 'sharedlibrary@master',
    retriever: modernSCM([
    $class: 'GitSCMSource',
    credentialsId: 'GIT_USER',
    remote: 'https://bitbucket.axisb.com/scm/inf/jenkins.git'
    ])
project_config = [
    branch: 'master',
    currentEnvironment: 'prodsandbox',
    regressionApi: 'business-loan-api-test',
    regressionUi: "maximus-regression-helm",
    new_dev: 'true',
    buildAgent: 'regression-test-agent-with-hostaliases-jdk17-newdev.yaml'
    ]
runBLRegression(project_config)
