pipeline{
  agent any
environment {
  PATH = "${PATH}"
}
stages{
    stage('terraform init'){
      steps{
        sh "terraform init"
      }
    }
  }
}
def getTerraformPath(){
  def tfVpc = tool name: 'terraform', type: 'terraform'
  return tfVpc
}
