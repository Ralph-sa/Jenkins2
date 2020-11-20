pipeline {
  agent any
  stages {
    stage('1') {
      steps {
        sh 
        '
        echo "Hello World"
        PID=$(pgrep "Unity")
        if [ -n "$PID" ];then
        echo "关掉当前的Unity进程 pid:$PID"
        KILL -9 $PID
        fi
        '
        echo '111'
      }
    }

    stage('2') {
      steps {
        sleep 1
      }
    }

    stage('3') {
      steps {
        echo '333'
      }
    }

  }
}
