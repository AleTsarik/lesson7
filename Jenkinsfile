//pipeline {
//    agent ('ubuntu') {
//      stage('install elk') {
//        docker run -d -p 9200:9200 -p 9300:9300 elasticsearch:7.17.7
//      }
//    }
//}

node ('ubuntu'){
    stage('Wshow Hello') {
        echo 'Hello World'
    }
    stage('install elk') {
//        docker{
            image 'elasticsearch:7.17.7'    
//        }
    }
}    
