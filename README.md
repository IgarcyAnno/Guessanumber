# Guessanumber
Guess a random number from 1 to 1,000

import random
target=random.randint(1,1000)
time=10
guess=eval(input('please input your answer:'))
while True:
    time=time-1
    if time<=0:
        print('you are running out of times')
        break
    else:
        if guess<target:
            print('your anser is less than the right one')
            print('warning!your left time(s) is:',time)
            guess=eval(input('try again:'))
        elif guess>target:
            print('your anser is larger than the right one')
            print('warning!your left time(s) is:',time)
            guess=eval(input('try again:'))
        else:
            print('you are right')
            break
