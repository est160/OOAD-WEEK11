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
 
 
 
 
 #code
 
title Study Class
 
 @startuml

[*] -up-> start.class

start.class -right-> introductory.talk

introductory.talk --> study.Content

study.Content --> half.break

half.break --> continue.class 

continue.class -left-> end.class

@enduml



                              PIC 3 Study Class



![](http://www.plantuml.com/plantuml/img/PKz13i8m3Bld5JaZjKz0a_O4ZeX3QJDMBRIeJG_xFLd5n0Gtsx5iPwZYYhGdWqHXmekqiEB8hbQudcvesikSiPkixoeS29eI7xEe8oOfEJGlkQnM72y0VnAQ7gK5Tin9ACaMTg3TC3kUxBsGquWlxYUljfWQVSe1VWJ3D6rZA8LzxA1Olti3)



#code

@startuml

title 7 ELEVEN

[*] --> 7e

state 7e 

state "7 ELEVEN Branch" as 7e {

  state "applying for a job" as applyingforajob
  
  state staff
  
  state head
  
  state unemployed
  
  applyingforajob --> staff
  
  staff --> head
  
  head --> unemployed
  
  unemployed --> applyingforajob
  
}

state NDoff

state "7 ELEVEN Headquarters" as NDoff {

  state manager
  
  state owner
  
  manager --> owner
  
  owner --> manager
  
}

7e -Right-> NDoff : Liaise

NDoff -Left-> 7e :Management

@enduml



                                   PIC 4 7 ELEVEN
                                   
                                   
                                   
![](http://www.plantuml.com/plantuml/img/NP6nhi8m34NtV8N5YDGPYU498Ien58Oti2060quRr2ObJOKGujznJLEWIzDxVAyJ9uice0zjLQfWGaamWpHBT-bMxQS7I98_c95YI-0AWUf_9z45Iu_sL4m0cwx-K02z0-kwl1kRWtOU42xkAAQ8cIApmSzVhGTL49u7qLggwjBTgKEZl9pmAwkra3xVBQ9_Mdo4rCOdUiOXjol7RSS3hxddjUKh8z_8H6Bxchn2YpdvGRkR5TLpsJCoMON45E_EzvZycxm8ZD_Dvv0PD0sfjqmoqa5U1kORoLLaWr8BicT-o1S0)


                              
                              
                              
                              
                              
                              
#code



                                   PIC 5

![]()


                             
