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
    stage('Test in dev') {
    }
    stage('Deployment to int') {
        ansibleTower(
            towerServer: 'Localhost',
            templateType: 'job',
            jobTemplate: 'CreateAPI',
            importTowerLogs: true,
            extraVars: 'stage: int'
        )
    }
    stage('Test in int') {
    }
}
