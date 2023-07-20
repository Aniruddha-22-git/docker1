pipeline{
  agent{
    label('built-in')
  }
  stages{
    stage('docker1'){
      steps{
        sh "git clone https://github.com/Aniruddha-22-git/docker1.git -b 23q3 /mnt/23q3"
        sh "docker run -itdp 8081:80 --name 23q3 httpd"
        sh "docker cp /mnt/23q3/index.html 23q3:/usr/local/apache2/htdocs "
        sh "docker exec 23q3 chmod -R 777 /usr/local/apache2/htdocs"
      }
    }
  }
}
