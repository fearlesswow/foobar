------
With one last roar of the escape pod's engines, you and your bunny companions jump to lightspeed. Congratulations! You've destroyed the LAMBCHOP, relieved the bunnies, gotten Commander Lambda off your tail, and saved the galaxy. Time for a little rest and relaxation back on Bunny Planet. Pat yourself on the back -- you've earned it!

Traveling through a nebula is a really bad idea, but with Commander Lambda hot on your tail, you don't have many options. Hopefully you can lose them once you're inside!

Oh no! You escaped Commander Lambda's exploding space station -- but so did the Commander, and Lambda is definitely not happy with you. Lambda is chasing you in a heavily-armed starfighter, while you and the bunny workers are stuck in these lumbering escape pods. It'll take all your wits and cleverness to escape such a hare-y situation, so you'd better hop to it!

Was that the sound of the spa facility imploding? You say a mournful mental goodbye to its sauna and massage tables. It's too bad - after all this scrambling, you really could use a nice relaxing day at the spa.

There are a lot of difficult things about being undercover as Commander Lambda's personal assistant, but you have to say, the personal spa and private hot cocoa bar are pretty awesome.

Excellent! You've destroyed Commander Lambda's doomsday device and saved Bunny Planet! But there's one small problem: the LAMBCHOP was a wool-y important part of the space station, and when you blew it up, you triggered a chain reaction that's tearing the station apart. Can you rescue the bunny workers and escape before the entire thing explodes?

As Commander Lambda's personal assistant, you get to deal with all of the paperwork involved in running a space station big enough to house the LAMBCHOP. And you thought Bunny HQ had too much bureaucracy...

Who the heck puts clover and coffee creamer in their tea? Commander Lambda, apparently. When you signed up to infiltrate the organization you didn't think you'd get such an up-close and personal look at these more... unusual tastes.

There are a lot of difficult things about being undercover as Commander Lambda's personal assistant, but you have to say, the personal spa and private hot cocoa bar are pretty awesome.

Awesome! Commander Lambda was so impressed by your efforts that you've been promoted to personal assistant. You'll be helping the Commander directly, which means you'll have access to all of Lambda's files -- including the ones on the LAMBCHOP doomsday device. This is the chance you've been waiting for. Can you use your new access to finally topple Commander Lambda's evil empire?

The latest gossip in the henchman breakroom is that "LAMBCHOP" stands for "Lambda's Anti-Matter Biofuel Collision Hadron Oxidating Potentiator". You're pretty sure it runs on diesel, not biofuel, but you can at least give the commander credit for trying.

The perks are definitely better as a Henchman than as a Minion. You're even allowed to sleep lying down!

You survived a week in Commander Lambda's organization, and you even managed to get yourself promoted. Hooray! Henchmen still don't have the kind of security access you'll need to take down Commander Lambda, though, so you'd better keep working. Chop chop!

Commander Lambda sure is a task-master, aren't they? You're being worked to the bone!

Success! You've managed to infiltrate Commander Lambda's evil organization, and finally earned yourself an entry-level position as a Minion on their space station. From here, you just might be able to subvert Commander Lambda's plans to use the LAMBCHOP doomsday device to destroy Bunny Planet. Problem is, Minions are the lowest of the low in the Lambda hierarchy. Better buck up and get working, or you'll never make it to the top...
------

So, my first clue that there was an additional, unlisted problem in Google's foo.bar is the wording and series of events that had happened. If we start with the encrypted message that's given after solving level 5, it appears to be a little bit off. After unencrypting using your username as the sign key, it lists:

b"{'success' : 'great', 'colleague' : 'esteemed', 'efforts' : 'incredible', 'achievement' : 'unlocked', 'rabbits' : 'safe', 'foo' : 'win!'}

As we can see, this is an array that gives us values variables below:
Success: great
Colleague: esteemed
Efforts: incredible
Achievement: unlocked
Rabbits: safe
Foo: win!

However, I noticed the array more accurately reads as a message:

"Great success, colleague. Esteemed efforts, incredible achievement, unlocked rabbits, safe win! foo"

Normally, in the English language, we wouldn't say that success is equal to great, as success is success. We'd more simply say that we were successful (Job: success, for example) and describe it as being great, but not equal to great. Applying this knowledge, we can flip "success" and "great."

Now, we're left with a confusing end message which states "Unlocked rabbits safe foo win!" which makes absolutely no sense in a string context. So, we perform the same operation at the end of the array that we did at the start, mirroring the flip with "win!" and "foo". This makes more sense anyways, as "foo: win!" follows the same sort of grammar structure failures.

We're left with the message "Great success, colleague. Esteemed efforts, incredible achievement, unlocked rabbits, safe win! - foo"

We can be certain that this is the accurate answer, because it now reads as a message signed by "foo" - aka, foo.bar. Foo isn't a game, it's a test, so there is no winning. There's just getting the answer right, or getting it wrong. It presents itself as a game with the opportunity to be hired directly by Google, but let me ask you this: do you really think that Google would recruit using an online program that has publicly posted answers and knowledge available? If they were going to recruit this way, each and every question would be unique as most code answers have a "most efficient/logical" answer associated with them, which would prevent Google from knowing which answers were legitimately obtained or if they were copied from others.

So, the question now is: What does "safe win" mean? And what does "unlocked rabbits" mean?

"Safe win" means that you won by completing all 5 of the tests. But what if I told you that there's a sixth test. Foo.bar already tests your ability to read, understand problems, apply mathematics, and use programming software to develop solutions. But what it doesn't test (knowingly) is your ability to think outside of the box and dig deeper into what's given to you. However, if you look at foo.bar's logo - this is exactly what they are actually looking for, and not necessarily your ability to program or understand math. 

On the other hand, "unlocked rabbits" potentially refers to the referral links they provide while completing problems. They provide two referral links, unlocked at separate intervals. It also means to work backwards, which is something that I will get to shortly.

I began to dig deeper, and realized a few things:

1. Upon opening the website after completing all 5 problems, you are given the message "With one last roar of the escape pod's engines, you and your bunny companions jump to lightspeed. Congratulations! You've destroyed the LAMBCHOP, relieved the bunnies, gotten Commander Lambda off your tail, and saved the galaxy. Time for a little rest and relaxation back on Bunny Planet. Pat yourself on the back -- you've earned it!"

2. There's two files in the directory: journal.txt and start_here.txt

This left me with even more questions, because they had cleared everything out of my home directory with the exception of these two files and the success message (or is it?). Why leave a file titled "start_here.txt" if all of the problems had already been solved?

That's right, it's an encrypted message. They're telling you to start with the journal file, and from there you're supposed to figure out the rest.

So, I opened the journal file, and realized further inconsistencies that now make the problem make more sense backwards, as opposed to forwards. With several clues along the way.

The first inconsistency actually relates to the "unlocked rabbits" statement. As you complete problems for foo.bar, more and more rabbits begin to appear on the screen hopping around in a box shape. So, we're not actually solving the problem. We're creating it. Which means that we need to work backwards to now free these rabbits.

The second inconsistency is how the first message starts with "Success!" while the last message states nothing about success. I knew at this moment that we actually had to start with the last journal entry and somehow work our way back to the first journal entry for us to actually be successful.

There's other hints along the way that this is the case. For example, "foo: win!" Means that foo had won, but as a player, we are supposed to beat the game and not let it get the best of us. "Rabbits: safe" actually means that the rabbits are now locked up and safe in a "prison" of some sorts, and we can be certain of this because the entire event called them bunnies and not rabbits. Using the word rabbits is almost insulting to them, as if they are being disregarded as what they truly are.

Further messages, such as "It's too bad - after all this scrambling you really could use a nice relaxing day at the spa" have led me to believe that I'm on the right track. There's also "better buck up and start working - or else you'll never make it to the top" (which is the last message, funnily enough, so if we work backwards we're working to the top which is "success!")

The question is: where do we start, what are we supposed to do, and why?

I think that Foo.bar is actually doing the opposite of what it says. Instead of freeing the bunnies, we actually imprisoned them. Throughout the challenge, it says that when one test is completed it is removed from the home directory. It doesn't say it's deleted though, and these submissions eventually get sent out to the recruiter (or so they say) once that clearance level is reached.

There are many clues and hints as to what needs to be done in order to access the recruitme command without providing the correct answers. For example, the line "Who the heck puts clover and coffee creamer in their tea?" is referencing the fact that javascript and python are used interchangeably in the source code. Commander Lambda could be thought of as the illuminati, because the theme of 3 is strong throughout these tests, but it's more likely that it's just Google. 

Very interesting problems, and it was fun and exciting to get to the bottom of what the test was actually about.
