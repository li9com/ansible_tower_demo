


node {
  stage("Checkout") {
    checkout scm
  }

  stage("Build") {
    echo "emplty for demo"
  }

  stage("UAT") {
ansibleTower credential: '', extraVars:
'''---
artemii_password: sdfsdf
artemii_username: dsfsdfdf
url: "http://yandex.ru"''', importTowerLogs: true, importWorkflowChildLogs: false, inventory: 'UAT', jobTags: '', jobTemplate: 'Show custom vars', jobType: 'run', limit: '', removeColor: true, skipJobTags: '', templateType: 'job', throwExceptionWhenFail: true, towerServer: 'tower.demo.li9.com', verbose: true
  }

 stage("Test_UAT") {
   echo "Empty for this demo"
 }

 stage("Approve") {
   input "Do you want to deliver new version?"
 }

  stage("PROD") {
ansibleTower credential: '', extraVars:
'''---
artemii_password: sdfsdf
artemii_username: dsfsdfdf
url: "http://yandex.ru"''', importTowerLogs: true, importWorkflowChildLogs: false, inventory: 'PROD', jobTags: '', jobTemplate: 'Show custom vars', jobType: 'run', limit: '', removeColor: true, skipJobTags: '', templateType: 'job', throwExceptionWhenFail: true, towerServer: 'tower.demo.li9.com', verbose: true
  } 

}
