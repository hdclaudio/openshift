pipeline {
    agent { 
        any { 
               image 'php:8.0.7-cli-buster'
               reuseNode true
               }
         }
    stages {
        stage('Ambiente') {
            steps {
                sh 'php --version'
            }
            // steps { 
            //     echo "====++++Instalando o Composer++++===="
            //     sh 'yum install php-cli php-zip wget unzip'
            //     sh 'php -r "copy(\'https://getcomposer.org/installer\', \'composer-setup.php\');"'
            //     sh 'HASH="$(wget -q -O - https://composer.github.io/installer.sig)"'
            //     sh 'php -r "if (hash_file(\'SHA384\', \'composer-setup.php\') === \'$HASH\') { echo \'Installer verified\'; } else { echo \'Installer corrupt\'; unlink(\'composer-setup.php\'); } echo PHP_EOL;"'
            //     sh 'php composer-setup.php --install-dir=/usr/local/bin --filename=composer'
            //     sh 'composer'
            // }
        }
    }
}
