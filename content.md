### Izveidot number guessiing speli ar Python programmesanas valodu

### Dokumenta saturs

### 1.APrakstit speli
Interesanta spele kas attista logiku.

### 2. Speles logika
dators nejauši ģenerē skaitli no 1 - 100 

spēles loģika ir crazy
```py
import random

repeat = True
while repeat:   
    number = random.randint(1, 100)
    guess = 0
    tries = 0


    while guess != number:
        if guess < number:
            print("Pamēiģini lielāku skaitli")
        else:
            print("Pamēiģini mazāku skaitli")

        guess = int(input("Uzmini sakitli: "))
        tries += 1
    else:
        if tries < 3:
            print(f"WOW! Tu uzminēji pēc {tries} reizēm!")
        elif tries < 7 :
            print(f"Nav slikti, tu uzminēji pēc {tries} reizēm!")
        else:
            print(f"Hm... vajadzētu trenēties uzminēji pēc {tries} reizēm!") 



            response = input("Vai tu gribi turpināt? y/n")
        if response == "y":
                repeat = True
        elif response == "n":
                repeat = False
                print("Paldies par spēli see ya!")
        else:
                repeat = False
                print("Paldies par spēli sigma")
```

