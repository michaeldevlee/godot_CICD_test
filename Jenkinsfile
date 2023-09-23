pipeline {
    agent any 
    environment{
        GODOT_EXE_PATH = 'C:/Users/Pencil/Desktop/Godot_v3.5.2-stable_win64.exe'
        GODOT_EXE = '/c/Users/Pencil/Desktop/Godot_v3.5.2-stable_win64.exe/Godot_v3.5.2-stable_win64.exe'
        PROJECT_PATH = '/c/Users/Pencil/Desktop/Mike/Programming/CICD/Jenkins-Godot/Test_Project'
        EXPORT_PATH = './docs'
        
    }
    
    stages {
        stage('Build') { 
            steps {
                sh '${GODOT_EXE} --path ${PROJECT_PATH} --export "HTML5" ${EXPORT_PATH}/index.html'
            }
        }
    }
}