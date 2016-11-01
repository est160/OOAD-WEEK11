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
