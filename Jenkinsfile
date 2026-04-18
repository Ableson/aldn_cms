pipeline {
    agent any
    
    stages {
        stage('拉取代码') {
            steps {
                echo '✅ 代码已拉取'
                sh 'ls -la'
            }
        }
        
        stage('构建') {
            steps {
                echo '🔨 开始构建...'
                // 这里添加你的构建命令
                // 例如：mvn build / npm install / docker build 等
            }
        }
        
        stage('测试') {
            steps {
                echo '🧪 运行测试...'
            }
        }
    }
    
    post {
        success {
            echo '✅ 构建成功！'
        }
        failure {
            echo '❌ 构建失败！'
        }
    }
}
