pipeline{
  agent{
    label('built-in')
  }
  stages{
    stage('docker1'){
      steps{
        sh "git clone https://github.com/Aniruddha-22-git/docker1.git -b 23q2 /mnt/23q2"
        sh "docker run -itdp 90:80 --name 23q2 httpd"
        sh "docker cp /mnt/23q2/index.html 23q2:/usr/local/apache2/htdocs"
        sh "docker exec 23q2 chmod -R 777 /usr/local/apache2/htdocs"
      }
    }
  }
}
