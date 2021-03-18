pipeline{
 agent{label "master"}
 stages{
  stage("Hello"){
   steps{echo "hello from jenkinsfile"}
  }
  stage("for the fix branch"){
   when{branch "fix-*"}
   steps{sh '''cat README.md '''}
  }
  stage("for the PR"){
   when{branch "PR-*"}
   steps{echo 'PR bababababbababa'}
  }
 }
}
