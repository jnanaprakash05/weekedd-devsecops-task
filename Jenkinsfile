node
{
  stage ("1.checking the files")
  echo "check the files"
  sh "ls -a"
  sh "mkdir -p test-folder"
  sh "touch test-folder/tset.sh"

  stage ("2.install some packages")
  sh "sudo yum update -y"
  sh "sudo yum install -y httpd"
  sh "sudo systemctl start httpd"
  sh "sudo systemctl enable httpd"
  sh "rpm -qa | grep httpd"
  sh "ps -aux | grep httpd"
}
