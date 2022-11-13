pipeline{
    agent any
    stages {
        stage('show Hello') {
            steps{
            echo 'Hello World'
            }
        }
    
        stage('install elk') {
            steps{
                sh 'wget -qO - https://artifacts.elastic.co/GPG-KEY-elasticsearch | apt-key add -'
                sh 'sh -c \'echo "deb https://artifacts.elastic.co/packages/6.x/apt stable main" > /etc/apt/sources.list.d/elastic-6.x.list\''
                sh 'apt update'
                sh 'apt install elasticsearch'
                sh 'systemctl start elasticsearch.service'
                sh 'systemctl enable elasticsearch.service'
            //    sh 'curl -fsSL https://artifacts.elastic.co/GPG-KEY-elasticsearch | sudo apt-key add -'
            //    sh 'echo "deb https://artifacts.elastic.co/packages/7.x/apt stable main" | sudo tee -a /etc/apt/sources.list.d/elastic-7.x.list'
            //    sh 'sudo apt update'
            //    sh 'sudo apt install elasticsearch'
            }
        }
    }
}
