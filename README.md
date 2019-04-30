# Front Running Capability (FRC)

When a game is close in score or tied pitchers are under an immense amount of pressure. Every next pitch can lead to their team being behind on the scoreboard. Pitchers are evaluated on whether or not they can keep the game tied or just keep it close enough for their offense to make up the ground. What about another situation though, when the game is basically in hand. Not even in hand, what about when their team is up by at least three runs and it’s too early to bring in a closer? Situations like this are when a pitcher can put the game away and secure the win. I look to find a new statistic that can highlight pitchers who can be early game closers, who perform best in situations where they are given at least a three run lead. 
	The data used is from Statcast, then compiled across an MLB season for every pitcher. The main metric used to evaluate a pitcher’s Front Running Capability are an accumulation of balls and strikes in the specific scenario outlined in the intro. Strikes are divided over balls for every relief pitcher, then the data frame is sorted from highest strikeout ratio to lowest and displayed alongside ERA for the season. The ERA is not based on the situation and instead from all of that pitcher’s pitches across any scenario. I wanted to put their season ERA side by side with strikeout ratio to see how closely the strikeout ratio compared to their ERA for the season. Along with this, I ran a linear regression on strikeout ratio and ERA to see how closely the two statistics compared. 

![alt text](https://github.com/EricOropezaelwood/Sabermetrics/blob/master/final/strikeout-ratio-linear.png)

As you can see from the linear regression plot, strikeout ratio is closely tied to how good or bad of an ERA an individual pitcher will have. I did the same test with a pitcher’s effective speed to see if I could combine speed and strikeout ratio to make FRC. The plot showed that this was not a good idea, it showed that effective speed was not a good indicator of a good pitcher in this specific scenario during a game. 
Given this, I decided to abandon combining the two statistics and chose to use strikeout ratio as the statistic to represent Front Running Capability. 
	While FRC and ERA are closely related, you are not able to determine how well a pitcher will perform when up by three runs. There is a certain mentality needed to keep a lead in a baseball game. If the pitcher gets complainant then the lead will vanish, along with the win. I believe this new statistic will highlight the best relief pitchers to put in as an early game closer. In the future, I can think of ways to improve this statistic. If there is a way to get information that doesn’t relate to ball velocity and pitch angles for a pitcher’s performance during individual outings on the mound then I believe adding that to strikeout ratio would produce an even better metric of which pitchers to rotate in for this situation. 


![alt text](https://github.com/EricOropezaelwood/Sabermetrics/blob/master/final/effective-speed-linear.png)
