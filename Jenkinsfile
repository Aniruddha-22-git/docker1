pipeline{
  agent{
    label('built-in')
  }
  stages{
    stage('stage1'){
      steps{
        //sh "yum install git -y "
        sh "yum install docker -y"
        sh "systemctl start docker"
        sh "systemctl enable docker"
        sh "git clone https://github.com/Aniruddha-22-git/docker1.git /mnt/23q1"
        sh "cd /mnt/23q1"
        sh "git checkout 23q1"
        sh "docker run -itdp 80:80 --name 23q1 -v /mnt/23q1:/usr/local/apache2/htdocs /httdp"
        sh "docker exec -it 23q1 chmod -R 777 /usr/local/apache2/htdocs"
      }
    }
  }
}
