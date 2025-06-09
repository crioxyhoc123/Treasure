print(r'''
____________________________________________________________________
 / \-----     ---------  -----------     -------------- ------    ----\
 \_/__________________________________________________________________/
 |~ ~~ ~~~ ~ ~ ~~~ ~ _____.----------._ ~~~  ~~~~ ~~   ~~  ~~~~~ ~~~~|
 |  _   ~~ ~~ __,---'_       "         `. ~~~ _,--.  ~~~~ __,---.  ~~|
 | | \___ ~~ /      ( )   "          "   `-.,' (') \~~ ~ (  / _\ \~~ |
 |  \    \__/_   __(( _)_      (    "   "     (_\_) \___~ `-.___,'  ~|
 |~~ \     (  )_(__)_|( ))  "   ))          "   |    "  \ ~~ ~~~ _ ~~|
 |  ~ \__ (( _( (  ))  ) _)    ((     \\//    " |   "    \_____,' | ~|
 |~~ ~   \  ( ))(_)(_)_)|  "    ))    //\\ " __,---._  "  "   "  /~~~|
 |    ~~~ |(_ _)| | |   |   "  (   "      ,-'~~~ ~~~ `-.   ___  /~ ~ |
 | ~~     |  |  |   |   _,--- ,--. _  "  (~~  ~~~~  ~~~ ) /___\ \~~ ~|
 |  ~ ~~ /   |      _,----._,'`--'\.`-._  `._~~_~__~_,-'  |H__|  \ ~~|
 |~~    / "     _,-' / `\ ,' / _'  \`.---.._          __        " \~ |
 | ~~~ / /   .-' , / ' _,'_  -  _ '- _`._ `.`-._    _/- `--.   " " \~|
 |  ~ / / _-- `---,~.-' __   --  _,---.  `-._   _,-'- / ` \ \_   " |~|
 | ~ | | -- _    /~/  `-_- _  _,' '  \ \_`-._,-'  / --   \  - \_   / |
 |~~ | \ -      /~~| "     ,-'_ /-  `_ ._`._`-...._____...._,--'  /~~|
 | ~~\  \_ /   /~~/    ___  `---  ---  - - ' ,--.     ___        |~ ~|
 |~   \      ,'~~|  " (o o)   "         " " |~~~ \_,-' ~ `.     ,'~~ |
 | ~~ ~|__,-'~~~~~\    \"/      "  "   "    /~ ~~   O ~ ~~`-.__/~ ~~~|
 |~~~ ~~~  ~~~~~~~~`.______________________/ ~~~    |   ~~~ ~~ ~ ~~~~|
 |____~____~__~_______~~_~____~~_____~~___~_~~___~\_|_/ ~_____~___~__|
 / \----- ----- ------------  ------- ----- -------  --------  -------\
 \_/__________________________________________________________________/
''')
print("Welcome to Treasure Island.")
print(" -> Your mission is to find the treasure. <-")
choice1 = input('You\'re at an island looking for treasure, '
      'Where do you want to go? '
      'Type "Dark Forest" or "Pixie Forest". ').lower()

if choice1 == "pixie forest":
    choice_2 = input('You got to the Pixie Forest, '
                     'you saw a fairy coming right at you.'
                     ' What do you do? Type "Talk" or "Ignore". ').lower()

    if choice_2 == "talk":
        choice_3 = input('The fairy talks to you and gives you powers.'
              ' What do you do with the powers that the fairy has bestowed you'
              ' use it for "Good" or "Bad". ').lower()
        if choice_3 == "good":
            print("You are the hero of the fairyland. Now you can\'t leave cause the land needs you."
                  " -> Remember your mission <- ")
        elif choice_3 =="bad":
            print("The fairies will get you and put you to the Prisoner of Azkaban")


    elif choice_2 == "ignore":
        choice_4 = input('Nothing happens but you continue to walk into the pixie forest. '
              ' Type "Continue" or "Stop" to see what happens. ').lower()
        if choice_4 == "continue":
            print("The wondering wizard from the dark forest sees you and kills you. Game Over.")

        elif choice_4 == "stop":
            choice_5 = input('Stop and rest but the wizard from the dark forest saw you'
                  ' What do you do? "Talk" or "Ignore" him. ').lower()
            if choice_5 == "talk":
             choice_6 = input(f'You {choice_5} to the wizard'
                                ' and the wizard was nice to you\n'
                                'so he gave you the key to the dungeon and treasure map\n'
                                'now you have entered the dungeon.\n'
                                'Which way you want to go? The "Prisoner of Azkaban" or "Owl House" ').lower()
             if choice_6 == "owl house":
                 print("Nothing happens you go to the owl house and live with them\n"
                       "-> Remember your mission.<- ")

             if choice_6 == "prisoner of azkaban":
                print(f"You went to the {choice_5}"
                          f" and then fought your way in\n"
                          f"got the treasure, and fought your way out. YOU WON!")
            elif choice_5 == "ignore":
                    print("Wizard kills you cause he saw you as a threat. Game over.")

if choice1 == "dark forest":
   choice2 = input(f'You have come to {choice1}, you see a wizard. What do you do?'
           ' "Talk" or "Ignore" him ').lower()

   if choice2 == "talk":
       choice3 = input(f'You {choice2} to the wizard'
             ' and the wizard was nice to you\n'
             'so he gave you the key to the dungeon and treasure map\n'
             'now you have entered the dungeon.\n'
            'Which way you want to go? The "Prisoner of Azkaban" or "Owl House" ').lower()

       if choice3 == "owl house":
           print("Nothing happens you go to the owl house and live with them\n"
                 "-> Remember your mission.<- ")

       if choice3 =="prisoner of azkaban":
           print(f"You went to the {choice3}"
                 f" and then fought your way in\n"
                 f"got the treasure, and fought your way out. YOU WON!")

   elif choice2 == "ignore":
       print("The wizard sees you as a threat so he kills you. Game Over XD")


