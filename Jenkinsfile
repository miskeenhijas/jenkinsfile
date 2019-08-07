pipeline {
agent none
stages {
stage ('Runnig linux command') {
agent {label 'linux'}
steps {
echo 'this is linux machine'     
sh '''    
touch /pipeline.me    
ls /
'''  
} 
}   
stage('Running windows commands') {
agent {label 'windows'}
steps {
 echo 'this windows slave machine'
 bat 'md E:\abc'
}

   
}


}

}

