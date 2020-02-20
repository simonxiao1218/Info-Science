#This is my journal for Info Sci


31/01/2020
1. What did we do? We were introduced to the basics of computational thinking and info science. We simulated a computers actions through making a sandwich. 
1. What did you learn? I learnt about the basics of computational thinking, which comes in 4 steps. I also learnt about the being precise and specific when creating computer algorithms.Computers do not have the common sense that we carry. So actions that seems automatic and obvious for us has to be stated explicitly for the computer.
1. What questions do you have? I am curious about how we can input instructions to a real computer.


6/02/2020

1. What did we do? We experimented with different commands in Processing to create different shapes. We experimented with colour, size, frequency and shape.
1. What did you learn? I learnt the basics of programming in Processing. i was able to create simple shapes. I learnt about background colours, fill colours, size and shapes.
1. What questions do you have? For homework, i have to create a dice image. I am still struggling a bit but I will research into the parts that I am unsure about.


10/2/2020

1. What did we do? We made our dice image into a dice simulator that was able to give us a random number of dots between 1 and 6 whenever we "rolled" (clicked) it. We then made certain numbers more or less likely to be shown, we challenged other groups to guess which side had the bias.
1. What did you learn? I learnt how to use the random feature, as well as applying bias and increasing or decreasing the probability of a certain outcome.
1. What questions do you have? While I have a basic idea of how to apply "bias," i am still not confident this the technique


13/2/2020
1. What did we do? We made our dice simulator more complex with more features. We added a counter that showed the total number of rolls. As well as a bar graph that shows the total number of rolls of each side. We also made your dice roll automatically, meaning we no longer had to manually "click" to roll. Below is the code for the dice.
1.what did you learn? I learnt to become more confident and familiar with the program, as well as how to add the extra features.
1.Towards the end, the bar geraph grew so large that it covered the dice. I wonder if there are any solutions to this issue.
# definition of variables
one_c=0
two_c=0
three_c=0
four_c=0
five_c=0
six_c=0

def setup():
    size (600,600)
    textSize(30)
    
def draw():
    x=0
    delay(10)
    mouseClicked()
    barGraph()
    
def mouseClicked():
    global one_c, two_c, three_c, four_c, five_c, six_c
    background(255)
    stroke(0)
    fill(255)
    rect(100,100, 400, 400, 10)
    stroke(255,0,0)
    strokeWeight(10)

    
    
    n=random(0,6)
    print(n)
    if 0<=n<1:
        circle(300,300,50)
        one_c = one_c+1
        print("Number of rolls for number one",one_c)
    if 1<=n<2:
        circle(200,200,50)
        circle(400,400,50)
        two_c+=1
        print("Number of rolls for number two",two_c)
    if 2<=n<3:
        circle(200,200,50)
        circle(400,400,50)
        circle(300,300,50)
        three_c+=1
        print("Number of rolls for number three",three_c)
    if 3<=n<4:
        circle(200,200,50)
        circle(400,200,50)
        circle(200,400,50)
        circle(400,400,50)
        four_c+=1
        print("Number of rolls for number four",four_c)
    if 4<=n<5:
        circle(200,200,50)
        circle(400,200,50)
        circle(200,400,50)
        circle(400,400,50)
        circle(300,300,50)
        five_c+=1
        print("Number of rolls for number five",five_c)
    if 5<=n<6:
        circle(200,200,50)
        circle(400,200,50)
        circle(200,400,50)
        circle(400,400,50)
        circle(200,300,50)
        circle(400,300,50)
        six_c+=1
        print("Number of rolls for number six",six_c)
        
def barGraph():
    fill(0)
    text(1, 50, 590)
    text(2, 80, 590)
    text(3, 110, 590)
    text(4, 140, 590)
    text(5, 170, 590)
    text(6, 200, 590)
    
    stroke(255,0,0)
    rect(53, 560-one_c, 10, one_c)
    stroke(255,224,32)
    rect(83, 560-two_c, 10, two_c)
    stroke(0,255,0)
    rect(113, 560-three_c, 10, three_c)
    stroke(0,0,255)
    rect(143, 560-four_c, 10, four_c)
    stroke(255,96,207)
    rect(173, 560-five_c, 10, five_c)
    stroke(96,255,128)
    rect(203, 560-six_c, 10, six_c)
    
    totalRolls=one_c+two_c+three_c+four_c+five_c+six_c
    text("rolls:",400,590)
    text(totalRolls, 475, 590)
    
20/2/2020

1. What did we do? We coded a 10 times 10 chessboard like image. We then altered the position of the black squares to create an optical illusion.
1. What did you learn? Today I was able to get more practice into programming basic shapes and adding colours. I was also able to program repeating patterns. This was able to save me a lot of time.
1. What questions do you have? This is not a direct question, but rather something i am unfamiliar with. I un still unfamiliar with the repeatuing patterns function. I think I need more practice programming basic repeating patterns.
