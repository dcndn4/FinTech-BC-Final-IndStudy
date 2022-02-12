# Robo Reminder
This project - a continuation of HW 10 AWS Unit 13 - its to support the process of a new accounting employee who has daily tasks that she doesn't want to miss on any day. So she has requested this robo-reminder, which she can run towards the end of the day, to make sure she hasn't missed anything. 

The more I think about it, the ongoing utility becomes clear. It's changing in my imagination to more of an ongoing process.

There is always a need to prioritize any free time amongst competing demands. It would be interesting to have a robo-reminder (RR) do that as possible. 

Here's how that would work (maybe a subsequent activity after this project iteration): I would launch the RR when I have a period of time free. It would ask some questions to determine tasks necessary and what the rest of the day looks like, and then it would present a triaged list of tasks for that period. And possibly a b-list for the later period that day as well. 

So I'm thinking to consider both sorts of functionalities.

Another set of functionalities would be the remind-other-staff set -- maybe would be a whole different robot though.. or a robot that informed the main reminder-robot. So details to work out yet, but this would be about all the accounting system elements that I need from other staff in order to do my job.. which they know I need, but they haven't provided within the specified time frame. Which is fine, of course. They're all very busy as well of course. So they can rest easy knowing I'll remind them when it's past time. 

But being aware of what isn't 'in' yet as soon as possible (always better to do sooner than later, so info is fresh in their minds etc..) is an ongoing challenge -- if I want until I actually need to urgently use it, then I might not have the right tone in the communication because it's throwing off my day, etc.. So I need to constantly scan kind of for things that are past due, and provide the most positive, constructive reminders possible to others. (This may need to be deleting sooner than later I'm realizing). So that robot aspect would be questions to me about what has been turned in, and when I answer no, then it provides me with a list potentially of reminders to send out. 



![Robo Helper](pending image)


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


# Technical Notes

Working on this project included setting up an AWS account, setting up an IAM user, and starting to learn about *very* carefully navigating around the enormous universe that is AWS. It amazes me that you can build something, leave it there, go search for a different function, work on that, search for the previous technology, pick that up again and combine those, and then the 3rd thing.. very well crafted. Still overwhelming!

I have the S3 bucket set as totally public, I'll leave everything in place until this assignment is graded or until there starts to be a charge on my account, whichever comes first (or for a week I'm thinking, at the longest). Then I'll go in and delete everything, to not accidentally incur hidden charges suddenly etc..


# Acknowledgements

I would like to first acknowledge the guidance and teaching of our FinTech Boot Camp Instructor, Garth Mortensen, our Student Success Manager, Angelica Baraona; and the whole team behind the curriculum, the logistics, the whole program. I also found the collective Stack Overflow wisdom essential as ever.

This project is for the purpose of my own ongoing learning, it is not a grading instance.

