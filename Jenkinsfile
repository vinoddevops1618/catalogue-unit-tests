// @Library('jenkins-test-library')

// def configMap = [
//     project: "roboshop",
//     component: "catalogue"
// ]

// echo "Triggering the library pipeline"

// if ( env.BRANCH_NAME.equalsIgnoreCase('main') ){
//     echo "checking later"

// }
// else{

//     testPipeline(configMap)

// }

// def configMap = [
//     project: "roboshop",
//     component: "catalogue"
// ]

// echo "Triggering the library pipeline"

// if ( env.BRANCH_NAME.equalsIgnoreCase('main') ){
//     echo "checking later"

// }
// else{

//     nodejsEKSPipeline(configMap)

// }


def configMap = [
project: "roboshop",
component: "catalogue"
]
echo "Triggering the library pipeline"

if ( env.BRANCH_NAME.equalsIgnoreCase('main') ){
    configMap["jiraProject"] = "ROBO"
    EKSMainPipeline(configMap)
}

else{
    configMap["jiraProject"] = "ROBO"
    nodeJSERSPipeline(configMap)
}