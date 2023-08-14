Postmortems:

is a procedure meant to aid you in drawing lessons from previous mistakes. It usually entails a debate or analysis shortly after an incident has occurred. Postmortems are usually conducted shortly after an occurrence or event and entail objective analysis and discussion. An artifact is created that contains a thorough explanation of exactly what went wrong to lead to the incident, a list of actions to do to stop it from happening again in the future, and a full description of what went wrong. Included in the discussion should be an evaluation of how your incident response procedure performed as a whole throughout the occurrence.
All website features, including the product listing, the shopping cart feature, and the payment procedure, were affected by the outage. Each user
Issue Summary: 
August 10, 2023, 4:30 p.m. to August 14, 6:00 p.m. (UAT), 
The website was a complete flop.
Users were unable to access the website during this period since it ceased responding.


Time Line 

Our monitoring system discovered the problem around 4:30 PM, and it immediately alerted the operations staff.
- 4:35 PM – An effort to restart the web application server by the operations team failed to fix the problem.
- 4:40 PM – Assuming there was a setup issue with the server, the team started looking into the situation.

- 5:00 PM — The team suspected a memory leak when further examination showed that the server's memory utilization was unusually high.

- 5:15 PM – The team began examining the application's code to find any probable memory leak reasons.

- 5:45 PM – After locating the memory leak in the code, the team started to develop a repair.

- 6:30 PM – The team restarted the web application after deploying the update. 


Misleading Investigation: 

The team spent a lot of time investigating since they first thought the issue was due to the server settings. This made it harder to find the root of the issue.

Escalation:

The situation was first addressed by the operations team, but when they learned the issue was with the application code, they escalated it to the development team.



Resolution:

The web application's code had a memory leak, which was found and rectified. Code optimization and best practices regarding controlling memory were part of the solution. Following patch deployment, the web application server was restarted, and complete website functionality was recovered.



Corrective and Preventative Measures:

The following remedial and preventative actions will be put into practice in order to avoid such problems in the future:
- Conduct routine code reviews to spot possible memory leaks.
- Put in place more stringent testing practices to find memory leaks before they affect production.
- Increase the server performance and resource use monitoring.
- Enhance operations team training and documentation to better prepare them to manage occurrences like these in the future.


certain tasks are:

- Completely examine the web application's source code.
- Create more automated tests to find memory breaches.
- Add more precise resource consumption statistics to monitoring tools.
- Give members of the operations team additional training on resolving web application problems.

