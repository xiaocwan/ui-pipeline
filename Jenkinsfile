

def runner_job_model = ""


def breakCurrentJob(message) {
  currentBuild.result = 'ABORTED'
  error(message)
}


node("ui-slave") {

  stage("Trigger Runner-v3 Jobs") {
    try{
      runner_job_model = readYaml text: env.FLEXY_JOB_MODEL
      println "runner_job_model"
    } catch(Exception ex) {
      breakCurrentJob("Fail to read RUNNER_JOB_MODEL as yaml, ${ex}")
    }






}