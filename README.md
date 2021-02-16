# Approximation-for-cubic-root
cube=8
epsilon=0.001
guess=1.0
increment=0.001
num_guesses=0
while abs(guess**3-cube)>=epsilon:
     guess+=increment
     num_guesses+=1
print('num_guesses= ',num_guesses)
if abs(guess**3-cube)>=epsilon:
    print("Failed on cube root of ",cube)
else:
    print(guess,' is close to the cube root of ', cube)
    
 # Approximation-for-square-root
 square=16
epsilon=0.01
num_guesses=0
low=1
high=square
guess=(high+low)/2.0
while abs(guess**2-square)>=epsilon:
    if guess**2<square:
        low=guess
    else:
        high=guess
    guess=(high+low)/2.0
    num_guesses+=1
print('num_guesses= ',num_guesses)
print(guess," is close to the square root of",square)
