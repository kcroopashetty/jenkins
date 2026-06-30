pipepline{
agent any
stages{
stage('clone repository'){
steps{
git branch : 'main'
url : 'https://github.com/kcroopashetty/jenkins.git'
}
}
stage('status'){
steps{
echo "succesfullly cloned github repo"
}
}
