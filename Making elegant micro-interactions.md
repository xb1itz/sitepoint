#Creating elegant micro-interactions#
Interaction design became a buzzword that relates to proper UX design process. If you won't make your website sexier with fancy animated interactions it is no go. You will loose your SWAG. 
However fancy interactions are not synonymous elegant ones. If you are creative like me, you occasionally want to show off by creating fancy-flying interactions just to make your website cooler. Though doing that, it is especially easy to screw up your entire user experience and make your website annoying or even harder to use.

![Elegant](https://www.dropbox.com/s/m66bjbu8nzs7nte/2752162749_843d508f47_b.png?dl=1)


##So what is a micro-interaction?
When user makes an input *(e.g. clicks, drags, types something)* your website reacts - well, that's an interaction. This is a way for users to communicate with your website, so it's like a dialogue between those two counterparts. When designing a flow how users behave on your website, you always to few choices how to implement interactions: 

 - **Navigation.** It's when users end up in a totally new state of a website. 
 - **Modal interaction.** It's when current state of website is frozen and some temporary state is displayed on top of it (e.g. "lightbox" gallery or confirmation dialog.) 
 - And you use a **Micro-interaction** when you want only a particular element of a page to react to user input - like show a drop-down menu or reveal more details of a product. 

##Why it is important
Face a fact! Minor, unnoticeable details deals a huge impact on great design and draws a line between just **"fine"** and **"awesome"** experience. Enriching your website with micro-interactions not only makes it more usable, but renders a positive emotions for users. Experiencing such emotions means more dopamine is consumed and this literally makes them more addicted to your website. 

##How do we make things elegant?
A website should feel like a concert of interactive interface elements working together to impress you. Elegance is the key criteria to make such impression. Though we can't express elegance in tech terms, we can use some logic hacks that helps us to create elegant interactions.   

###Key rule - No teleportation
The idea is simple - always use transitions when you changing something on page. That means there shouldn't be any instant snap-cuts on your GUI. Every appearing, disappearing or transforming element should be implemented with easing or/and animation. This helps users to focus their vision on the areas you want them to. And of course this creates a feeling of elegance and consistent flow.   

![No teleportation](https://www.dropbox.com/s/c3m4sw8f8byvjv1/no-teleport.png?dl=1)

###Trigger placing
You usually use the same switch to turn on and off lights in your room. The same concept applies to controls toggling something on your site. If some control triggers some state of an element - the same control should rollback that state. Furthermore, according to [Fitts' law](http://en.wikipedia.org/wiki/Fitts%27s_law) such controls requires close to zero effort to rapidly switch something on and off.  

![Trigger placing](https://www.dropbox.com/s/4gmkbi46fgqew23/trigger.png?dl=1)

###Transition origin and direction
Transitions always have a trigger. It's the control element that users use to set of a transition. At a time of interaction user is always focused on trigger. So it is necessary that transition originate from or nearby it. If you start transition too far away from trigger, user could just miss it and the flow will break.  
Furthermore a transition should propagate from trigger to the position where you want to focus users' attention. The trick is simple - you lead users eye from trigger to the spot where he should make his next move. This way users won't loss their focus and will be right on the track where you want them. 

![Transition origin and direction](https://www.dropbox.com/s/d9ru6b0vvipm8vm/transition-origin.png?dl=1)

###Natural transition timing
Transition timing defines how long animation of transition is playing. The major problem of timing is that there is no silver bullet to get it right. If you make transition too long - it will create a pain if users repeat the same interaction often or rapidly. On the other hand, if it is too short, it won't make the effect or will feel unnatural. All you can do is to evaluate the transition by your eagle eye. The best advice is not to make all transitions with same timing all over your site. Just play around and find the right balance. Also note that even a difference of **0.05s** matters. 

![Natural transition timing](https://www.dropbox.com/s/44sx5j89y59n4c6/transition-timing.png?dl=1)


###Transition rollback (feeling of control)
Sometimes it happens that users change their mind quickly, in the middle of transition. In case this happens transition responsiveness is critical. If user cancels the last interaction (e.g. clicks trigger button twice) the animation of transition should be **instantly** reversed. If it is not, user automatically looses the feeling of control. Furthermore you are making user think that he did something wrong.   

![Transition rollback](https://www.dropbox.com/s/8vpl43yve8t2obo/transition-rollback.png?dl=1)

###Focus on next action in series
This particular tip is dedicated for interactions where users perform a sequence of actions. When designing such sequence, you should avoid any unnecessary interactions and always set focus on the next control in sequence. The most basic example of such interaction is an *[edit]* button that opens a form and magically focuses on the first field so that user does not need to click it manually.

![Focus](https://www.dropbox.com/s/o6sbbazqa9qc3zy/focus.png?dl=1)

###Necessity of action Feedback 
Users should always recognize a time when interaction is done. If some kind of interaction does not obviously change website appearance, you should always consider implementing visual feedback that tells users *"Hey you, it's done!"*. In situations you skip that, users tend to repeat the same action multiple times, thus making a mistake and even corrupting something precious. 

![Feedback](https://www.dropbox.com/s/iayfkhuc2ib0o33/feedback.png?dl=1)

##Applying these hacks
In short, you can use these hacks as cheat-sheet for implementing micro-interactions on your website. It should help you design the details of interaction before you implement them. However, there is a good chance that you won't make them perfect at first time. In that case you will need to tweak them according to the situation - so be prepared to play around a little. 
Aaaaand... there just the last tip for take away. In general, the more interaction surrenders to the laws of real world physics, the more it feels natural and elegant. Have animating fun! 