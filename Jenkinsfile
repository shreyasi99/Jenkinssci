pipelineJob('job-dsl-plugin') {
  definition {
    cpsScm {
      scm {
        git {
          remote {
            url('https://github.com/shreyasi99/Jenkinssci.git')
          }
          script('''
       pipeline {
            agent any
                stages {
                    stage('Stage 1:Build') {
                        steps {
                            echo 'Ready to build'
                        }
                    }
                    stage('Stage 2:Deploy') {
                        steps {
                            echo 'Ready for deployment'
                        }
                    }
                }
            }
          ''')
        
          branch('*/main')
        }
      }
      lightweight()
    }
  }
}
