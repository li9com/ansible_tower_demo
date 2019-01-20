


node {
  stage("Checkout") {
    checkout scm
  }

  stage("AnsibleTowerStage") {
ansibleTower credential: '', extraVars: '''
artemii_password: sdfsdf
artemii_username: dsfsdfdf
url: http://yandex.ru
''', importTowerLogs: true, importWorkflowChildLogs: false, inventory: '', jobTags: '', jobTemplate: 'Show custom vars', jobType: 'run', limit: '', removeColor: true, skipJobTags: '', templateType: 'job', throwExceptionWhenFail: true, towerServer: 'tower.demo.li9.com', verbose: true

  }
}
