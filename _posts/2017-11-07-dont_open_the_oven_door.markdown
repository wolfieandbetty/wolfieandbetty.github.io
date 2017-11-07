---
layout: post
title:      "Don't Open the Oven Door!"
date:       2017-11-07 23:20:45 +0000
permalink:  dont_open_the_oven_door
---


Old habits and old learning can get in the way of assimilating new knowledge!

Let's say that you've been cooking for 10+ years. You KNOW how to cook. In fact you're a good cook - people compliment you on the tasty meals you crank out with ease and skill. But you've never made a Souffle' and you get a hankering to invite some friends over and impress them with a beautiful meal. So you google several recipes and rather than read all the tedius instructions you look at the ingredients list and scan through the instructions. Seems pretty easy. After all you are an accomplished cook. While the Souffle' is cooking you decide to open the oven door and have a peek to make sure all's good. And almost immediately after you close the oven door, your beautiful Souffle' deflates and is just an unappealing mass of eggs and cheese. You'd have been better off making an omelet! But you get angry because sheesh - you beat the eggs properly and were exact in your measurements with all the ingredients. The person who wrote the recipe is an idiot!

Thing is - you skipped over the part of the instructions that told you NOT to open the oven door while it was cooking. 

This was my experience with Methods. I haven't written code in a very long time and in my old APL programming days I wrote subroutines regularly. So when I read about methods I was like "Oh - it's a subroutine. I understand booleans and how to structure conditional statements and I get looping. Easy peasey, I know how to do this". But then I started writing methods and they didn't give me the results I expected. And after much head scratching and head banging I realize that the key reason for an unintended outcome is that I keep opening the oven door and screwing it up.  My oven door opening mistake was using PUTS.  I was sticking PUTS in at the end of my methods to see if my variable assignments or conditional statements were giving me the results that I thought they should give. The problem is that the PUTS at the end of my methods result in the method evaluating to NIL. Not good.

I finally figured it out after going back through previous course material READING it and finally the lightbulb went off and I did a little test with IRB:

def speak (phrase="I don't know")
phrase==phrase.upcase
end


speak
=>false


BUT! If I open the oven door to get a peek (insert a PUTS) I get this:

def speak (phrase="I don't know")
phrase==phrase.upcase
puts phrase
end



speak
I don't know
=>nil

Doh!!  Lesson learned. Read instructions with beginner's mind, don't substitute real understanding about how to get the results you are aiming for by assuming that old knowledge will solve a new problem. There will be many reasons that you may not get the results you expect but hopefully, if like me you made this same mistake, you can put this one behind you.
