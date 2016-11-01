# OOAD-WEEK11
State Diagram

#code

@startuml

Title Hard Working 

State sleep

State "wake up" as wakeup

State "go to work" as gotowork

State "finish work" as finishwork

State "go home" as gohome



sleep -right-> wakeup

wakeup -right->gotowork

gotowork -down-> finishwork

gohome -right-> finishwork

gohome -up-> sleep

@enduml

                    
                                            PIC 1 Hrad Working



![](http://www.plantuml.com/plantuml/img/RL0n3iCW4DjvnIaxNwWoTc-bpaXS0OLm20xb-oKXWLOg2pO-sy2SMIKkgnVYwTWZt5NIyAAqk610Y0ShHiWUCLvasjI2KE84AiEEov0C0HDirNweXfXsqlMt2oxRCT3upqYDiBJYwT-XgEku0SZaZ6LvwxLjx-UZxq8WDMsXEhwRMkn8-wULM8NptJC6NR_e0m00)



#code

@startuml

title Playing Game

[*] --> PlayingGame

state PlayingGame 

state "Playing Game" as PlayingGame {

  state Human
  
  state "Internet cafe" as Internetcafe
  
  state Game
  
  state "Shop owner" as Shopowner
  
  Human --> Internetcafe
  
  Internetcafe --> Game
  
  Game --> Shopowner
  
  Shopowner --> Human
}

@enduml



                                        PIC 2 Playing Game
                                        
                                        
 ![](http://www.plantuml.com/plantuml/img/NL112W8n3Bpd5M6Fmdv1zgRU18_Y8MZKXJOhtImYujzjqzrIXHuwavd9a6vK2Zfv1w2zEiQzerSlDzoGPpYkJjYswuKqBXgKQmPXvfhQso2DFwet86RTTl8a1JKxKGx2YcUwPjl29ABeR7an7Ux30uUdS317WeQY8ZxROCt_ecfeypdL6YPS1vM_JNBh3q37Sea7-m80)
