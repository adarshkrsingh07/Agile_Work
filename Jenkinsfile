pipeline 
{
    agent any

    stages 
    {
        stage('Building') 
        {
            steps 
            {
                echo 'Building the Application'
            }
        }
        stage('Testing') 
        {
            steps 
            {
                echo 'Testing the Application'
            }
        }
        stage('Deploy') 
        {
            steps 
            {
                echo 'Deploying the Application'
            }
        }
    }
    post
    {
        failure
        {
            emailext body: 'This pipeline is for Agile Exp 10.', subject: 'Agile Practicle', to: 'adarshkrdixit@gmail.com'
        }
    }
}
