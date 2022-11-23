pipeline
{
    agent any
    parameters
    {
        choice(choices: ["Male", "Female"], description: "Choose Gender", name: "chGender")
        string(defaultValue: "", description: "Enter Name", name: "name")
        booleanParam(defaultValue: "false", description: "Give Consent", name: "consent")
        string(defaultValue: "", description: "Enter Age", name: "age")
    }
    stages
    {
        stage("Deployment")
        {
            steps
            {
                echo "Enter your Name : ${params.name} \n"
                echo "Enter your Age : ${params.age} \n"
                echo "Choose your Gender ${params.chGender} \n"
                echo "Do you give your consent for this Information? ${params.consent}"
            }
        }
    }
}