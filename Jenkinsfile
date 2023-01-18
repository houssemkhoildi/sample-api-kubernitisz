pipeline {
  agent {
    dockerfile {
      filename 'hou'
    }

  }
  stages {
    stage('hou') {
      parallel {
        stage('hou') {
          steps {
            sleep(time: 15, unit: 'MICROSECONDS')
          }
        }

        stage('kh') {
          steps {
            node(label: '15')
          }
        }

      }
    }

    stage('ikram') {
      parallel {
        stage('ikram') {
          steps {
            echo 'hello ikram'
          }
        }

        stage('') {
          steps {
            dir(path: 'user/hou') {
              echo 'user'
            }

          }
        }

      }
    }

  }
}