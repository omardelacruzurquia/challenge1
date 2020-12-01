# challenge1

# Ejecución
    sh challenge1.sh output => muestra las variables x default
    sh challenge1.sh create => crea los recursos necesarios para el deploy : docker image && cluster
    sh challenge1.sh destroy => elimina todos los recursos creados : docker image && cluster
    
# Indicar el archivo json que contiene las credenciales en la variable 
  GOOGLE_APPLICATION_CREDENTIALS="/tmp/sa1-294.json" #!!!!!!!!!!! MANDATORY
  en el archivo challenge1.sh
  
# Acceso a la "app"
  kubectl get svc # Tomar nota de la IP PUB Externa asignada al servicio "api"
  http://<IP>             =>> Hello World
  http://<IP>/greetings   =>> Hello World : Hostname <platform.node()>
  http://<IP>/square/<N>  =>> Number : N
                              Square : N*N
  
