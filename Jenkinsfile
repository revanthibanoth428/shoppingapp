node {
     stage('get code from Github') {
         git branch: 'main', url: 'https://github.com/revanthibanoth428/shoppingapp.git'
     }
     
     stage('build java code using maven') {
         def mavenHome = tool name:"maven 3.9.6", type:"maven";
         def path = "${mavenHome}/bin/mvn";
         sh "${path} clean package";
     }
}
