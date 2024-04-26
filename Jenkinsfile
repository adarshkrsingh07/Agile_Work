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
        stage('Launch') 
        {
            steps 
            {
                echo 'Launching the Application'
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
