@Library('jenkins-shared-library') _
// env.COMPONENT="cart"  Passing the variable like this or below anything is fine.
env.COMPONENT="catalogue"
env.SONAR_URL="172.31.41.5"
env.NEXUS_URL="172.31.45.41"
env.UPLOAD_STATUS=sh(returnStdout: true, script: "curl http://${NEXUS_URL}:8081/service/rest/repository/browse/${COMPONENT}/ | grep ${COMPONENT}-${TAG_NAME}.zip || true")
nodejs ()