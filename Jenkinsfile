pipeline{ 
    agent any

    stages{ 
        stage("pulling the source code"){ 
            steps{ 
                echo "code pulled"
            }
        }

        stage("building the image"){ 
            steps{ 
                echo "image built"
            }
        }

        stage("running the image"){ 
            steps { 
                echo "running image container"
            }

        }

        stage{ 
            steps{ 
                sh """

                    sudo apt-get install nginx -y 

                    sudo systemctl enable nginx 


                    sudo systemctl start nginx






                    """
            }
        }
    }
}