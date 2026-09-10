# practice-bartout
# Adam Bartout
## Jason Statham

** Jason Statham ** is my favorite actor, he's known for playing different <baction> movies, which I love. I grew up watching him playing racing, rescue, shooting and spy movies. He is an ** important ** actor to me who has contributed to building my character<br>


---

## Favourite movies and songs

-**Favourite movies by Jason Statahm**

1. The transporter
2. Crank 
3. The Italian Job

-**Favourite songs**

- "Passionfruit"
- "We Are One (Ole Ola)"
- "Waka Waka"


Click here to know what my favourite city is: [My Favourite City](MyCity.md)

---

## Jokes from People I Know

A couple of jokes that people in my life always say.

**Connor**, my coworker, always says:

> You know what they say, you get paid by the hour not the job.

**Dau**, my friend, always says:

> I don't skip leg day, I skip everything, it's called nap time.

---

## Code Snippet: Minesweeper

This is a recursive example from the Minesweeper game. When a cell with no adjacent mines 
is picked, the `cellPicked` method recursively reveals all of its neighboring cells, which 
is how clicking one empty spot in Minesweeper can open up a whole blank area at once.

​```java
public class MineSweeper
{	private int[][] myTruth;
	private boolean[][] myShow;
	
	public void cellPicked(int row, int col)
	{	if( inBounds(row, col) && !myShow[row][col] )
		{	myShow[row][col] = true;
		
			if( myTruth[row][col] == 0)
			{	for(int r = -1; r <= 1; r++)
					for(int c = -1; c <= 1; c++)
						cellPicked(row + r, col + c);
			}	
		}
	}
​```

[Minesweeper Recursion Example — Source](https://www.cs.utexas.edu/~scottm/cs307/javacode/codeSamples/MineSweeper.java)
