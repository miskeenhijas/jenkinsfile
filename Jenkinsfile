pipeline {
agent none
stages {
stage ('Runnig linux command') {
agent {label 'linux'}
steps {
echo 'this is linux machine'     
sh '''    
touch /pipeline.me    
ls /root/home
'''  
} 
}   
stage('Running windows commands') {
agent {label 'windows'}

 echo 'this windows slave machine'

   
}


}

}

