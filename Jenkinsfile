node {
    stage('Deployment to dev') {
        ansibleTower(
            towerServer: 'Localhost',
            templateType: 'job',
            jobTemplate: 'CreateAPI',
            importTowerLogs: true,
            extraVars: 'stage: dev'
        )
    }
}
