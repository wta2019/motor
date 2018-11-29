# motor
definition(
    name: "Motor App",
    namespace: "motor_open",
    author: "Cesar Montoya",
    description: "controla Puerta!",
    category: "My Apps",
    iconUrl: "https://s3.amazonaws.com/smartapp-icons/Convenience/Cat-Convenience.png",
    iconX2Url: "https://s3.amazonaws.com/smartapp-icons/Convenience/Cat-Convenience@2x.png",
    iconX3Url: "https://s3.amazonaws.com/smartapp-icons/Convenience/Cat-Convenience@2x.png")


 preferences { 
    section ( "Abrir la Puerta:" )  ) {
        input "switch1" , "capability.switch", required: true  
    } }


def someEventHandler ( evt ) {
     // ejecutar el controlador  tres segundos a partir de ahora
 
runIn ( 3 * 1 , handler  )
 

  }

 def handler () {
     switch1.off ()
 }
