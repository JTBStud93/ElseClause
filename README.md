# ElseClause
Write your understanding of the else clauses using comments and examples (at least 5 examples) to the instructor and describe them in your own words to the best of your knowledge. Put your work to GIT. Submit the GIT url to canvas. 

Since "If Statements" are meant to find the "Truth", anything that isn't gets put into the "Else Clause". Setting up the Else Clause is in the same format as you would write an If Statement.

Before you can start, you must ALWAYS have this:

void Start ()
{

#1 In the first example, I'm using the double equals sign (==), which means to compare data on both sides. Since 7 - 5 is indeed 2, this statement is true; but using any other number not shown in this example would result as false, or an error. Alternatively for the Else Clause, I could type 'print("Error");' but the Debug Error function I used will make the software (i.e. Unity) tell you an error has occured on purpose.
    
    if (7 - 5 == 2)
    {
        print(2);
    }
    else
    {
      Debug.LogError("Your answer is incorrect.");
    }

#2 (This next example was from a previous class,) Knowing that "If" looks for true statements while the "Else" looks for false ones, using an exclaimation mark "!" in a variable or function will filp it around. Now "If" is looking for false statements and "Else" will look for true statements.
    
    public bool canEat;
    
    Let's say a bird can eat, while a chair can't.
    
    if (!canEat)
    {
      print(this.name + " can eat.");
    }
    else
    {
      print(this.name + "can't eat.");
    }
    
    So in Unity (for example) will say, The bird can't eat, but the chair can.

#3 In this example, I'm using the "Not Equal" sign (!=). It helps to identify the compared data that are NOT the same.
    
    public string myName = "Tanner1993";
    
    if (myName != Dorris1903)
    {
      print(myName);
    }
    else
    {
      print("Please reenter your username correctly.");
    }

#4 (Another example that was from today's class,) It shows that "health" or "100" is greater than "0", and the "%=" works just the same as division (using "/" or "/="), but it seeks the remainder. HOWEVER, in this example, it's showing that "2" is being divided by "0", and that results as an error (so including an error message would be appropriate for this case). Now if it was "0" divided by "2", the answer would simply be "0".
    
    //Health
    public int health = 100;
    
    if (health > 0)
    {
      health %= 2;
      print(health);
    }
    else
    {
      Debug.LogError("You can't Divide by Zer0.");
    }


#5 The next example is from the book on page 56, but an alternate example will be present instead. Turns out that you can actually put another If Statement within an Else Clause.

    if (4 * 4 == 8)
    {
    Console.Writeline (Does Not Compute);
    }
    else
    {
      if (4 * 4 == 16)
      {
        Console.Writeline (Computes);
      }
    }

}
