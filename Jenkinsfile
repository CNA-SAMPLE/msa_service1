node {
     stage('Clone repository') {
         checkout scm #repository�� jenkins workspace�� clone
     }

     stage('Build image') {
         app = docker.build("demo/demo:$BUILD_NUMBER") #docker image build �� �̸��� teicahe/jenkins:�����ȣ ����
     }
}