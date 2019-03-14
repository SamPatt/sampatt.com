---
layout: post
title: Ancient Game Now in a Blockchain: The Story of CryptGo
---

Cryptocurrency advocates are often quick to point out that the technological innovation of the blockchain isn't only useful for handling a currency. Much discussion revolves around how blockchains will be used eventually, but so far only a few projects (such as Namecoin) use a blockchain with something other than currency as the primary purpose.

I happened to find such a project recently. It uses a blockchain to allow users to play a popular board game peer-to-peer. The project is only a few days old, and very rough, but as a proof of concept I found it worthy of documenting. I've also interviewed the author to understand more about the project.###Board game and Blockchain?

I stumbled across the project a few days ago on 
[reddit](http://www.reddit.com/r/CryptoCurrency/comments/20adji/boardgame_go_inside_of_a_cryptocurrency_moves_are/) with the headline:

>Boardgame "go" inside of a cryptocurrency. Moves are transactions which miners verify. Small python program, fast to install.

I happen to enjoy playing Go, also known as wéiqí, igo, or baduk. If you're not familiar with the game, you should 
[check it out](http://en.wikipedia.org/wiki/Go_%28game%29). It's older than chess, and extremely popular in east Asia.

My favorite board game merged with a cryptocurrency? I couldn't resist, so I visited the 
[Github repository](https://github.com/zack-bitcoin/CryptGo). It was a brand new project, with one contributor, Zack-Bitcoin, the creator who had posted on reddit.

I checked out the code, and it seemed legitimate, if a bit haphazard. I cloned it, and with a bit of help from other redditors, eventually got it running. It runs by downloading the blockchain, which is a history of moves played in the game, and by running a gui that is accessible by pointing localhost at port 8090.

It didn't work at first. There is a cost associated with playing a game, and a cryptocurrency that needs to be mined to facilitate the games. It appeared that there were only three people who had installed the new project, myself, Zach-Bitcoin, and another redditor named Archer. Sending the coins needed to play the game wasn't built into the interface yet! To get around that, the creator made the default wallet accessible to myself and Archer to get us started (he needed testers badly).

It worked! I sent along my public address to Archer, and we started the first game.

###Gameplay

Here's what the interface looked like.


[![Blockchain Go](http://samuelrpatterson.com/wp-content/uploads/2014/03/Blockchain-Go.png)](http://samuelrpatterson.com/wp-content/uploads/2014/03/Blockchain-Go.png)

I played black. My opponent was new to Go, and as we played we chatted and I gave pointers (on a separate interface, it doesn't support chat).

The gameplay was very crude. You clicked to place your stone, which sent the move into the blockchain. Since the game continually monitors the blockchain, the gameplay can take place fairly quickly, but the interface didn't automatically display my opponents moves. I had to click refresh each time, which got annoying. There was also no counter to display captured stones, nor to indicate whose turn it was.

By using the chat, Archer and I were able to make it through an entire game. Here's the result of our game.


[![CryptGo4](http://samuelrpatterson.com/wp-content/uploads/2014/03/CryptGo4.png)](http://samuelrpatterson.com/wp-content/uploads/2014/03/CryptGo4.png)

If you're familiar with Go, you know that selecting dead groups and counting territory is in integral part of the endgame. Archer and I couldn't figure out how to end the game and determine the count. We could have done it manually, but didn't bother since it wasn't a close game. We had to wait for the 5 minute timer to expire, and me to hit "Win game," which appeared to be intended for people who abandoned gameplay.

The result was anticlimactic, when we refreshed it said "The game does not exist," not giving a count or even mentioning that I'd won.

It was clear that this was the very beginning of the project, which needed significant work if it were going to be useful for playing Go. I later learned that our game was one of the first ever played with the program.

Archer and I had found many bugs and had lots of suggestions for improvement, so I contacted the creator, Zack, to let him know. He's tried making some of the changes, and the project was on hold for a day until some of the bigger bugs were worked out.

He appreciated the help and suggestions, and we struck up a conversation. I offered up the name CryptGo for the project, which he liked and adopted.

###Interview with Zack-Bitcoin

By this point, I felt the project was worth writing about, so I asked Zack if I could send him along a few questions, which he kindly agreed to and answered.


**Are you a student? What's your occupation? How did you learn programming?**


>I was a student studying Physics at UCSB. I was one of the top physicists in my class, in my third year, when I dropped out to work on this project. I have enjoyed making small mathematical programs since I was 13 or so. I fixated on finding prime numbers, and other such problems.


**Where did you get the idea for this program? Why create it?**


>DAC=Distributed Autonomous Corporations are beautiful to me. I love the lack of hierarchy. Most people think that cryptocurrencies can only be used for money, but really, distributed computers can compute anything that a normal computer can compute. I want to build big DACs which will replace our governments, schools, businesses, etc.

Whenever possible, I prefer making fun things rather than non-fun things. As cool as bitcoin is, it is not fun.


**Are you aware of any other blockchain based games? How long did it take to create?**


>I heard about huntercoin, but have not looked at it. I have spent a little under 2 months working on CryptGo so far. What is unique about CryptGo, is that it is written completely from scratch. Almost every other altcoin is a copy of bitcoin.


**How many people have been played so far / how many games completed?**


>3 games have been played. You vs Archer. Me vs Archer, and my dorm-mate vs me.


**Where do you hope CryptGo ends up? Do you see the blockchain setup being used for more games in the future?**


>I have immediate plans to put the game amiraa into a blockchain. There is a turned-based videogame called "civilization". the most recent version is "Civ V". I think that I could build something similar into a blockchain. I would love to do poker, but I think it might be impossible.

I see blockchains being used for lots of purposes in the future. I see them replacing all email, social networking, gambling, datastorage... I think that blockchains will be used for all cases of homesteading, and for determining property rights of land, and objects. I think that blockchains will replace armies for national defense, because a blockchain-based assassination market will be created.

I want to change places like Las Vegas and Washington DC into useless relics. I hope that blockchains will cause every instance of management, or hierarchy, to become so extremely non-optimal, that people will adapt away from those modes of existence.


**Any other projects you're working on?**


>I am currently working on a reddit clone blockchain. It is being called "NEWScoin" right now.


**Any general thoughts or questions I've missed?**


>CryptoGo is written in the functional style of coding. Most people talk about "object oriented" coding today. Functional coding is a very un-popular alternative to object oriented. Functional coding is nice, because the best functional coders are able to write more than 10 times faster than the best object oriented coders. It is the only reason I was able to write a cryptocurrency in 2 months. I learned from 
[this book](http://mitpress.mit.edu/sicp/).

I am an 
[agorist](http://agorism.info/), which is a type of anarchist or voluntaryist. We believe that actions like voting do not make the world any better. We think that the current system is too broken to fix from within.

Agorists think that a person who works a government regulated job is unable to understand how anarchy could work. Mark Twain 
[explains](http://paulgraham.com/cornpone.html) the phenomenon well.
Agorists think that building up the black market, and giving people opportunities for non-regulated jobs, is the best way to improve the world. Every additional person working a black market job is one more person who can think about anarchy rationally.

I am interested in DACs because I think this is the easiest way for me to create legal black-market jobs.

I want my children to grow up in a better world than the one that I grew up in.


###Novelty or New Direction?

It's clear that CryptGo isn't ready for the limelight. If there is a demand at all for this type of project, it would need a larger development team and a whole lot more testing and building. As I post this Zack is trying to work out a way to fix problems with forking and mining, and the roll-out hasn't been smooth.

It's unclear that there are enough Go players who are unsatisfied with their current online play that they would use something like this.

Regardless of the slim possibility that CryptGo will be widely adopted, projects like CryptGo (and another blockchain game, 
[Huntercoin](http://huntercoin.org/)) are worth watching.

Zach's vision of a world where blockchain technology eliminates hierarchies seems unrealistic. But the fact that a relatively inexperienced programmer created this project himself in a short period of time proves that the experimentation with blockchain technology has very low barriers to entry. If blockchain projects receive even a fraction of the effort that is dedicated to the app economy, who knows what new projects we might see?