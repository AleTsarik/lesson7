pipeline {
    agent ('ubuntu') {
      stage('install elk') {
        sk 'docker pull elasticsearch:7.17.7'
//          docker run -d -p 9200:9200 -p 9300:9300 elasticsearch:7.17.7
      }
    }
}
