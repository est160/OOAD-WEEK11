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

@startuml

title Chart Show TV

[*] --> Programs

state Programs 

state Programs {

  state "Open TV" as Open
  
  state "Select channels" as Selectchannels
  
  state "normal program" as normalprogram
  
  state "morning News" as morningNews
  
  state movie
  
  state cartoon
  
  state "affternoon News" as affternoonNews
  
  state Documentary
  
  state "game show" as gameshow
  
  state series1
  
  state "evening news" as eveningnews
  
  state series2
  
  state "Close TV" as Close
  
  Open --> Selectchannels
  
  Selectchannels --> Close
  
  Selectchannels --> normalprogram
  
  normalprogram --> normalprogram
  
  normalprogram --> Close
  
  normalprogram --> morningNews
  
  morningNews --> Close
  
  morningNews --> movie
  
  movie --> Close
  
  movie --> cartoon
  
  cartoon --> Close
  
  cartoon --> affternoonNews
  
  affternoonNews --> Close
  
  affternoonNews --> Documentary
  
  Documentary --> Close
  
  Documentary --> gameshow
  
  gameshow --> Close
  
  gameshow --> series1
  
  series1 -->Close
  
  series1 --> eveningnews
  
  eveningnews --> Close
  
  eveningnews --> series2
  
  series2 --> Close
 
  Close --> Open
  
}

@enduml




                                   PIC 5 Chart Show TV
                                   
                                   
                                   

![](http://www.plantuml.com/plantuml/img/ZPHDImCn48Rl-HL3Zq8F-WEaKCygLBo8Xx1ETnVoKPAqHSJ_RZutcMmFGg7pFlFEP3kJxSuwRjnP2iRSx0J2Vl8Q3fE-mjix-xZxXEts4LwD7WsNbdcxmqK2wy4F0qXeyt92vNjiW5i8SSqSKE3WO9YuKYXiT2HMKFKgRIGNS4e7H6j2cLIdr4RDQeHdlAQM6GIzkAI-pBYemVzMhPiduyUZGwCygsqg8vsUz72MgFpulclzo2M2zSEBbK45iUGjcXdjVVNZ1UCpgt9O1gezALKzrAgzq1RBQAFmEV-94m_hMWsJWkWfTJTI_O29_gUZj5zdw5eQHUfwNXONlpjd8NMTEIA-bgrsIW6fkv6YksyKAUnvSnrAIFm4DbSbHO4MPuEw6zCeqhldpPrAKUlsD5snmFAhotuPsw7wydyLVm00)


                             

#Activity Diagram

#code

@startuml

title  School


start

while (wake up?)  is (No)

  :Wait wake up for go to school;

endwhile (Yes)

  :take a bath;
  
  :dressed up;
  
  :Go To School;
  
stop

@enduml




                                      PIC 1 School
                                      
                                      
                                      
![](http://www.plantuml.com/plantuml/img/DOwn3i8m34HtVyMDxI_GWMviB20Xna0CYIYuYbtrzt536E-T_NIZMYYsl2SYopOnSBed4OzK6w8rPSVT6bwCPTxtG5PqH-c9WDqbP4Fhy922fy04MYK34NzY4rnPVo-sNGVSWgN1yuPYOLMExlYJW-0iRKjbQZ8JZUxpiLy0)  




#code

@startuml

Title Cubed machine doll.

(*) --> "Insert coin"

    --> "Wait for coin fully"

if "Control Machine" then

  -->[true] "Machine Active"
  
  --> "Clamp Doll"
  
  --> "End Process"
  
  -right-> (*)
  
else

  ->[false] "Night Coins"
  
  -->"End process" 
  
  --> (*)
  
endif

@enduml  



                                     PIC 2 Cubed machine doll
                                     
                                     
                                     
                                     
![](http://www.plantuml.com/plantuml/img/JP11QyCm38Nl-XKFdxP2znDAHxR33Yqx37OeExY9t1WKEzZAOFz-IfRG-IBpdlJfeMDLNtGQXEWZgZ2QwSeT1j_sCJ6wBF94zB1xn7v_W7jBbOkYpJ4v8jXRv4yV5I6NnK2OH7xCZW6koKbB5fp-W0xQSvedRUwYPU8lkDN3SwlncvsPj78RySE85mlnNtrD7TvBRhdMJIxnrgjv5dHMM2elImwNuErlIyvp1nhBL--i1JMkg8s_CL8N0z7Hgftd5m00)





#code

@startuml

title Triffic LED 


skinparam backgroundColor #BBBBBB

skinparam activity {

  StartColor Blue
  
  EndColor Green
  
  BackgroundColor orange
  
  BorderColor Yellow
  
}

start

:RED LED ACTIVE;

:YELLOW LED ACTIVE;

:GREEN LED ACTIVE;

stop

@enduml




                                PIC 3 Triffic LED
                                
                                
                                
                                
![](http://www.plantuml.com/plantuml/img/NO_12i8m44Jl-nKB_eLUQceeGh5GYz9ZRDCIcYPbcoeY_hk9LT0kUthCpiv4enFafbu3EEMqn89KqwWAKxv301WxPGP1eiUBgBgMx6Jgs6fBk6Bl-PM8ogchSdTy020UW_EiPNgIdlZbt_E4f3GpOmjdIyAq7pspL4kQUIcrjhV0d_vhS0TOvpvdoBgDY_s9RpmfUPfcvmLCSiuF_snqTW28fAbz_HS0)





#code

@startuml

title After School 

start

:Have a dinner;

:take a bath;

if (Playing Game?) then (yes)

  :__Have a Fun__!!!;
  
else (no)

  :Not Have a Fun;
  
endif

:Jogging; 

note left: 30 minute

if (Read Novel?) then (yes)

  :__Relax__!!!;
  
else (no)

  :Not Relax;
  
endif

if (Take your homework?) then (yes)

  :__Finish__!!!;
  
else (no)

  :Not Finish Yet;
  
endif

:Take your homework;

:Sleep;

stop

@enduml




                               PIC 4 After School
                               
                               
                               
![](http://www.plantuml.com/plantuml/img/VP4zJyD038Pt_mfdIpSajcIWB0KnLAXbOOeEukHETUpguXJoxxbha01HTJpVe-Vrnteq5sqQ6C22CU5zPnHn_-vL6G7Etm3LepiHEco32CKw5SmTSk7DcK_Fq67vp6uEqkE36-XkXUP9i9nfN04WLatphTXCqZH5KTIf2iGZOIcwC5ir_A4MGDhGfRWdxViahrDBeaR8r5c5jpSu19cCbWvsv5hSweduKlwEs7rUYpu3lrEpyoNFEUiKqUj07neFbzoR867qr-GBWQzaV-Rwhy_BtJFHiSxRroF0Ei7fGby0)




#code

@startuml

title Go Home


start

:After school;

:Wait for Last Train;

if (You are Late?) then (yes)

  fork
  
    :__Worry__!!!;
    
  fork again
  
    :Train to gone!!;
    
  fork again
  
    :Find taxi for go home!;
    
  end fork
  
else (no)

  :don't worry;
  
  :relax;
  
endif

:Go To home;

stop

@enduml





                                   PIC 5 Go Home
                                   
                                   
                                   
                                   
![](http://www.plantuml.com/plantuml/img/VL2xZi8m4EptAoRLXLz82aB3NN4b4gAAh6EJM6Uyo5u4-VlRc0Cw94lMxZmqErrMb_Ho2aJgDJ0-1LzoOY8g256p6PGJyiya4bgRzyuh1aduTbcnIyv7M_i1zK4kS8aDK5wle1D7r3Fd5H4MnQzzze2cx_UIqjptLLMrPVNFW1lDxyahxb31A97VKxS-7g7kvaksKJ3P6Iy56_g8m24pwYWbLtEK-A6uBddQkrkJEBXR6Kpc1plQQjdTBTkb6JaJTOPPSNy0)
