pipeline
{
    agent any
    parameters
    {
        string(defaultValue: "", description: "Enter your Name", name: "Name")
        string(defaultValue: "", description: "Enter your Age", name: "Age")
        choice(choices: ["Male", "Female"], description: "Choose your Gender", name: "Gender")
        booleanParam(defaultValue: "false", description: "Do you give your consent for the information?", name: "Consent")
    }
    stages
    {
        stage("Deployment")
        {
            steps
            {
                echo "Name : ${params.Name} \n"
                echo "Age : ${params.Age} \n"
                echo "Gender: ${params.Gender} \n"
                echo "Do you give your consent for this Information? ${params.Consent}"
            }
        }
    }
}