# Getting Better at Coding

## DRY

Now that are a lot of acronyms and rules for best coding practices. If you want you can look at [NASA's Ten Rules for Developing Safety-Critical Code](https://en.wikipedia.org/wiki/The_Power_of_10:_Rules_for_Developing_Safety-Critical_Code) which is
definitely an interesting read but following these rules for non mission critical code can be extra.

The one coding acronym/rule I follow constantly is **D**on't **R**epeat **Y**ourself (DRY). I am constantly looking at my code and thinking of ways to not repeat myself. Could I wrap this in a function? Am I looping over the same data twice? Is this if statement redundant?
There are a billion ways to repeat yourself in code and it takes practice to start eliminating some of these common repeats.

One example I have from work is a script I built to setup my database with the correct users. The script uses an Active Directory API call to find a user's managers info. The script took about 20 minutes to run as there are hundreds of these API calls and they each take a
second or two. I was thinking to myself "I feel like there are a ton of redundant API calls." And I was right. Let's say a manager has ten employees. This script was making the API call for the same manager ten times for the same information. So I implemented
memoization to cache the results. My script went from taking 20 minutes to around three minutes.

You gotta be always thinking to yourself "there has to be a better way"

## Six Month Rule

There's this Youtube video I watched a weeks [How I Accidentally Beat League of Legends](https://www.youtube.com/watch?v=sP2ml9V212c&t=2269s). The video entails a Youtuber that was challenged to reach the rank of Platinum (there's different ranks based on how good you
are at the game, Silver, Gold, Platinum, Diamond, ect) before the end of the year. Giving him about six months to go from Bronze rank to Platinum rank. He struggled a lot but every single day he focused on improving. While this sounds corny, getting better at a
video game is more than just playing the game every day. If you really want to improve you should study up, watch replays of your matches and see what you did wrong, try new things, potentially coaching, ect. At the very end of the six months with about a day to go,
he managed to achieve Platinum rank.

I truly believe in six months you can truly become competent in something if you put your mind to it. I've heard a lot of students show concern about their programming competence and to me, the best way to change that is to really hone in and become better.

## Computer Scientist vs Software Developer

Do any of the two people reading this document know what Computer Science stands for? To put it simply it's the study of computers. You're not getting a Software Development degree, you're getting a Computer Science degree. Now some people might think I mean this
as an insult towards the Computer Science degree. What you learn during your CS degree is worth its weight in gold. That being said I still think students should put an emphasis on teaching themselves a little more Software Engineering on their own or through internships.

## Gen AI

During school, using Gen AI like ChatGPT is a massive No No. When you start working, the dynamic is completely different. Now I'm not saying you should be able to use ChatGPT on your homework. That would be stupid. I just want to talk a bit about using ChatGPT for coding
help.

Now I would suggest 95% of the time avoiding using GenAI when developing, especially if you're new. It is easy to fall into the trap of copy and pasting ChatGPT answers back and forth until you have something that kind of works. Even if your code works perfecty, there's a
lot of downsides to over relying on Gen AI. You won't understand your code nearly as well and you learn far less are the two biggest downsides. Now if you're a little more advanced in programming you can lead your questions more and focus what you want ChatGPT to write
more so it's more advantagious. There are also times where you encounter a really weird error and it can take 30 minutes of Googling or reading Documentation when ChatGPT can figure it out in seconds.

The Spark Notes of this section is after you graduate, I would use Gen AI to assist in coding sparingly but also not avoid it entirely.
