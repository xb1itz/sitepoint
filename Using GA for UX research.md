
#5 ways you can use GA for your UX research
When users are visiting your website without you watching you probably feel like leaving a child alone at home while you went to a store for bottle of milk. You don't know how they are behaving and if they are doing their chores right. 
Same here. Your users can be misdirected, lost or don't know what they are doing at all on your site. Furthermore they can break something or get hurt themselves by making bad decisions (e.g. delete some important data of theirs). We are doing [Dragdis](http://dragdis.com) - it's a tool designed for creative professionals to make them be more creative by helping collect and organize inspirations. If you're designing for creative industries you especially have to think about interactions and make every usage scenario perfect - we like to say "Your path has to have flow" 

![enter image description here](http://i.memeful.com/memes/MExb36w/Ancient-Aliens-Guy.jpg) 

However in reality it is impossible to predict every use case or thought that your user can imagine when he sees your design, so we need to get feedback about our user behavior as soon as possible to make appropriate changes to our design. Furthermore if you're dong startup, your goal is to close feedback loop for Lean UX as rapid as you can. So in this article I will cover basics how to get feedback (statistical data) about your UX as soon as you roll out your design. 


##Why Google Analytics 
Though Google Analytics is a tool mostly designed for marketing purposes, it offers some cool features that can be salvation for UX researcher when he needs to get insights right here and right now without putting too much effort. Here's why we naturally selected GA as our main UX research tool: 

 - While most UX tools usually damages your budget, basic GA account is free of charge. You no need to go for Premium, because the data you get for free is quite enough to learn your users.
 - The level of flexibility GA provides is almost ultimate. You can set it up to observe usage trends, actions performed, track errors... you just can't name it all - it's up to you what answers you want to get. 
 - Data visualization of your data is one of better ways to understand it. Here in GA you can slice your data in various ways and had it presented and compared in charts. 	
 - It's so easy to setup. You have to paste just a small snippet of javascript and you are ready to go.

Of course, GA is not an ultimate tool. Tasks that require off-site data such as eye tracking or observations during usability testing should be conducted with other UX tools. Although you are free to use GA to gather data that is collectable within your website in the browser.

##Basics on GA tracking structure
Before you begin with your user analysis with GA, you should be familiar with basic levels of GA tracking. In your GA, you can have multiple Accounts, Properties and Views:

 -  Top level is Account. You should use it to separate **individual projects** or websites you want to track, like example.com or test.org
 - Properties offer you the way to **separate concerns in a single project**. Lets say *example.com* have some *public pages* for user acquisition and *internal pages* for already registered users - these two should go into separate properties since they have different purposes. In that way your user flow and metrics will be clearly distinct.
 - View is just another level of your data separation. It is useful if you want **filter and additionally process** incoming data from your website to see different contexts of it.    

##Things to track
When you are setting up your GA or configuring a report, first you should know what you want to discover. These are 5 simplest tracking features for basic analysis. 

###1. Standard Pageview tracking for starters
By default GA provides you standard tracking code that observes how your user is navigating and some parallel data that tells something about your users (what kind of tech does they uses, how they did get yo your site). Basic tracking allows you to answer these simple questions:

- Where users enter and where do they leave your website 
- Where users go in your website and what routes they take
- What technology users use *(mobile or desktop, screen resolution, OS, etc...)*  

Since standard tracking is more oriented for marketing, usually you will be able to get shallow insight from it, because it tracks only actual pages and not the interactions you want to know about. However you can easily make it more powerful by pimping up your tracking code with virtual page hits to observe user behavior in more detail. Virtual page hit means you have to set it up manually by calling tracking function when user performs action what you want to track. In example if you want to know if user opens another tab or loads another gallery item *that does not reload your page*, you can just add a single line of code in your javascript, that tells GA to track the particular interaction as a page hit.

    ga('send', 'pageview', '/your-custom-pageview');

###2. Behavior flow
The pearl you get when you had your pages set up is the **Behavior flow** (Under *Behavior* section). It is GA a report that tells how exactly your users are navigating within your website. 
This particular report is useful in these cases:

- To analyze the how users behave at particular point of your flow
- To see what happens before/after users take a particular step or visit particular page   
- In what sequence users perform different interactions
- If users are taking any unnecessary steps or returning to previous states for any reason
- What steps in your scenario fail mostly (users does not behave as you intended)  

Once you get there, select view type *"Automatically grouped pages"* and you will see all you user flow in visualization like the one below. If you click on a particular page (or step), you you will be able to Highlight a traffic through that page or set it as starting reference for all visualization *(menu option Explore traffic through here)*   

![enter image description here](https://www.dropbox.com/s/047owtlvf99vzdx/bahavior-flow.jpg?dl=1)


###3. Funnels are awesome
Funnels an Goals are features designed to observe your most sensitive data, it is if and how your website fulfills its purpose. **Goals** in GA usually represent your website objectives and **Funnels** are predefined order of steps how your users reaches goals. 
Goals are set up in *Admin* section of GA for each view individually (In other words, you can have different goals in different context for same website). For the beginning you should set goals for every objective of your website, like *"Order completed"* or *"User registered"* - this will tell GA how to calculate conversions ans you will have fine performance reports.
Funnels on the other hand are the real treasure here - you can define up to 20 steps for each goal and later analyze the performance of each of these steps. Each step represents a page hit or virtual page hit so only your imagination is the limit how you will use them, but the best practice is to create a funnel step for every possible point in your behavior flow, where users are able to abandon your scenario. 
These are the cases where you should use Goals and Funnels:

- To track how your website is performing to complete its objectives
- To know the points of your scenario where and why it fails
- To monitor overall performance of your scenario 

One you set up your goals, you will be able to use reports in *Conversions* section. **Goal flow** report will offer you same sort of insights as *Behavior flow*, though from perspective of goal completion - here you will be able analyze how users are jumping between funnel steps and see where they leave your funnel or jump back into it. Here you can simply spot the flaws if your scenario logic and easily see the points where your users get lost.

![enter image description here](https://www.dropbox.com/s/uueg4s1l7wpfhqp/goal-flow.jpg?dl=1)

Another powerful report is **Funnel visualization** where you will see all your funnel performance in single view - it will show how much each step is effective (how many users pass it successfully towards a goal) and where users go if they leave your funnel at a particular step. 

![enter image description here](https://www.dropbox.com/s/u91983rn3xrjavc/funnel.jpg?dl=1)

*Funnel visualization* differ from *Goal flow* in a way that *Funnel visualization* report "fills in" steps if users are skipping them and represents a Funnel as straight forward scenario, where *Goal flow* report shows how users actually navigates between steps.  

###4. What features your users are grinding
In fluent UX details and micro-interactions matters a lot, though usually they don't belong in navigation and page tracking. Here GA Event tracking comes to help. Event in GA represents a standalone action that your users are taking, so it is perfect to track such interactions as Context menu opening or List view change. All events are custom and each event have 4 properties, that you define by yourself:

- Category is just a value for grouping events (e.g. Index page events)
- Action is a short name that represents event itself
- Label (optional) user to track additional text data
- Value (optional) user to track additional numeric data that can be used as a metric in custom reports

To track an event, you need to add different line of code, similar to pageview tracking. E.g.:

    ga('send', 'event', 'Category', 'Menu click', 'Menu item title', 100);
    
All Event reports can be accessed under *Behavior -> Events* section. Most useful report here is **Top Events** where you can see what action your users performs most usually. If you want to see all events listed in a single plain, just select *Event Action* as your secondary dimension and if you select view table by **Performance** to visually represent intensity of every action.

![enter image description here](https://www.dropbox.com/s/c0vklzw3v8607z7/events.jpg?dl=1)

###5. Timing matters
There will be a time when you will need to track time and answer the fallowing questions: 

- How quickly users can reach their goal in your website
- How much time some operations or action takes.
- What points of your website keep users waiting 

To provide you with answers to these questions GA has implemented a feature called **User timings**. It is another custom hit type designed to measure time - how long things take in your website. 

GA itself does not provide a timing function, so the trick is that you will have to measure a time by any means you have *(e.g. simple timestamp comparison)* and after that just provide timing data in custom hit tracking code, where you have to specify 4 parameters:

- Category is just a value for grouping your timing events (same as simple Events)
- A short name that represents event itself
- Time in milliseconds
- Label (optional) user to track additional text data
 
    ga('send', 'timing', 'Category', 'Watched video for', 1000, 'Some custom text');


You will be able to analyze all your tracked timings in **User Timings** report  under *Behavior -> Site Speed* section. Same as in Event report you will be able to see all your timing events in single view if you select *Timing Variable* as your secondary dimension.

![enter image description here](https://www.dropbox.com/s/umq95axkq4mi6wm/timings.jpg?dl=1)

##Some general tips
These 5 features basically can collect you a bunch of data, but it in the end it only matters how you are going to analyze it. You do not have to implement all of these trackers only because you can - they are here to answer a questions and collect feedback, so just try starting from asking what what you want to know see what you can learn from GA.   
