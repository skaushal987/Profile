pipeline
{
    agent any
    parameters
    {
        string(defaultValue: "", description: "Enter Name", name: "name")
        string(defaultValue: "", description: "Enter Age", name: "age")
        choice(choices: ["Male", "Female"], description: "Choose Gender", name: "chGender")
        booleanParam(defaultValue: "false", description: "Give Consent", name: "consent")
    }
    stages
    {
        stage("Deployment")
        {
            steps
            {
                echo "Enter your Name : ${params.name} \n"
                echo "Enter your Age : ${params.age} \n"
                echo "Choose your Gender: ${params.chGender} \n"
                echo "Do you give your consent for this Information? ${params.consent}"
            }
        }
    }
}