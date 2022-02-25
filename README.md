![Robo Helper](https://github.com/dcndn4/FinTech-BC-Final-IndStudy/blob/main/Images/istockphoto-1333625894-170667a.jpg)


# Robo Reminder
This project - a continuation of HW 10 AWS Unit 13 - and even though it hasn't been that long, feels like forever ago! How does this all work again? Yikes.

This project is to support the process of a new accounting employee who has daily tasks that she doesn't want to miss on any day. So she has requested this robo-reminder, which she can run towards the end of the day, to make sure she hasn't missed anything. 

The more I think about it, the ongoing utility becomes clear. It's changing in my imagination to more of an ongoing process.

There is always a need to prioritize any free time amongst competing demands. It would be interesting to have a robo-reminder (RR) do that as possible. 

Here's how that would work (maybe a subsequent activity after this project iteration): I would launch the RR when I have a period of time free. It would ask some questions to determine tasks necessary and what the rest of the day looks like, and then it would present a triaged list of tasks for that period. And possibly a b-list for the later period that day as well. 

So I'm thinking to consider both sorts of functionalities.

Another set of functionalities would be the remind-other-staff set -- maybe would be a whole different robot though.. or a robot that informed the main reminder-robot. So details to work out yet, but this would be about all the accounting system elements that I need from other staff in order to do my job.. which they know I need, but they haven't provided within the specified time frame. Which is fine, of course. They're all very busy as well of course. So they can rest easy knowing I'll remind them when it's past time. 

But being aware of what isn't 'in' yet as soon as possible (always better to do sooner than later, so info is fresh in their minds etc..) is an ongoing challenge -- if I want until I actually need to urgently use it, then I might not have the right tone in the communication because it's throwing off my day, etc.. So I need to constantly scan kind of for things that are past due, and provide the most positive, constructive reminders possible to others. (This may need to be deleting sooner than later I'm realizing). So that robot aspect would be questions to me about what has been turned in, and when I answer no, then it provides me with a list potentially of reminders to send out. 

With this work I'm planning to again utilize the Amazon Lex function for the chat box, the s3 buckets to hold the icons, and the lambda functionality to screen/process the data, adding to the knowledge acquired earlier.  

# Task List - Accounting/Finance employee of business

[]  Coding of all transactions for day reviewed, any corrections communicated and confirmed

[]  Costs per product line items updated (weekly)

[]  In-kind donations booked to expense and donation, so costs included in strategic planning

[]  Cash Flow forecast prepared for tomorrow /n

[]  Dashboard metrics prepared for tomorrow


# Task List - Accounting/Finance contractor hired by entrepreneur to help with their personal and business finance

[]  Year End Cycle - Pay Pal 1099 form - reconcile to internal records

[]  Monthly Cycle - Sales Tax review of any internet purchases from small vendors - record transactions for reporting

# Logic/Decision tree

To really complete this and make it work well, the lambda program would be a bit complex. It would take in the answers to the questions about what needed to be done today still; and based on the date, it would draw from it's internal programming regarding other tasks. It would also incorporate the amount of time available during this 'free time' session, and the percentage likelihood of there being a second 'free time' period later in the day. 

From all of that info, it would instantly provide a list of 3-5 tasks that were most important in the current period.

I don't know that I'll get that all done any time soon, but it seems like an instance of the journey being more important than the destination. 

# Questions

I will be noting questions along the way, to check off as I discover things during this process, or for future continued explorations.

[] Is there a built-in time function within Lex or Lambda or something, so that my Robo-Reminder will always already know the date? I will need for it to know if it's week one of the month vs. week two vs. week three, and hopefully the day of the week as well. If there is not that built in, then I would need to have that be part of the dialogue. 


# Technical Notes

## Region:
I am continuing to work in the 'Oregon' region, as we were told that one had the set of functionalities that was the best fit for our activities - and am continuing with those same activities.

## Bucket setup (for slot images.. I think..):
[] Versioning - enabled
I'm worried that this might be one of those things that trips into more costs, but sounds like could be useful to keep multiple versions and not  lose anything accidentally. So I'll try it, and just closely monitor the costs dashboard. 

[] Tags - used for tracking costs more closely.. 
Since I live in accounting land, this sounds like a really good idea to me, but from the documentation scan I did, there's a lot to it. I think I'll have to hold off for now. 

[] Encryption - also sounds like a great value-add, also more in-depth than I have the appetite for, so skipping for now (leaving as disabled).

## Amazon Lex:
Aspects of Amazon Lex that I'll be working with include:

Bot -- the visible outcome that interacts with the user to achieve a goal

Intent Name -- the request that the bot user is making to the bot (naming the goal)

Slot -- these are the details of the request that the user is making

Slot type -- Description of the type of variable that is being used for each slot - numeric, date, string, etc..

Sample Utterances -- the wording that the user may use in expressing their intent

Lambda program -- the connective tissue between the sample utterances, and the resulting actions of the bot. We used a python variant of lambda, noting that it was quite a different animal than the python language that we had been used to. I'm saving that part for when I've become more familiarized. 

The three types of functionality that the lambda function can provide include:

* Initialization (dialog code hook)
[*] Validation (dialog code hook)
[~] Fulfillment (fulfillment code hook)

Validation will come in to play in terms of timing of tasks, and confirming what day it is, when the various deadlines are, etc..

I'm making use of the example bot to get back in the swing of all this - very helpful! Much appreciated. Working through that reminds me that the bot (using the data in the slots only) replies the way it thinks it is supposed to, regardless of the text it is receiving. It doesn't actually recognize or process the actual content provided at all. 

The functionality required to have the bot respond specifically to various text content aspects is the lambda functionality. I'm working my way towards reviewing that again soon. 


## Termination:
My notes from that first AWS homework/class period indicated that it was optimal to terminate services, but that's just too much work right now. Hoping that my usage will be minimal enough that I can skip that step and still not incur any costs. So far A-okay!

# Acknowledgements

I would like to first acknowledge the guidance and teaching of our FinTech Boot Camp Instructor, Garth Mortensen, our T.A. Roberto Salazar Reyna; our Student Success Manager, Angelica Baraona; and the whole team behind the curriculum, the logistics, the whole program. I also found the collective Stack Overflow wisdom essential as ever. In addition, I'm starting to work through the 'AWS Certified Cloud Practitioner - Study Guide -Foundational  (CLF-C01) Exam' text by Sybex (Wiley). And I have the 518 page Amazon Lex guide, so there's that. 

Additional resources that have been provided or that I've come across in my process include the training resources from Deloitte's digital initiative, and these videos on AWS workings: [AWS Free Tiers](https://youtu.be/7z4O-zZ6O4U), [SageMaker Setup](https://youtu.be/LJu74lRnpHM).

I'm also more widely exploring readme formatting etc.. And also: I'm very glad I saved as many notes and path markers etc.. as I did at the time. At this point, I wish I had saved more of course. But every little bit helps.

This project is for the purpose of my own ongoing learning, it is not a grading instance.

