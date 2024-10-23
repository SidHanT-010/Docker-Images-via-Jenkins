pipeline {
    agent any
          stages {
                stage(&#39;Build Docker Image&#39;) {
                                                    steps {
                                                          script {
                                                          dockerImage = docker.build(&quot;&lt;your-username&gt;/docker-images-via-jenkins&quot;)
                                                                  }
                                                            }
                                                      }
                  stage(&#39;Run Docker Container&#39;) {
          steps {
                              script {
                                dockerImage.run(&#39;-d -p 7070:8080&#39;)
                                      }
                              }
                    }
              }
          }
