<h1>SQL Applying Filters to Queries</h1>


<h2>Description</h2>
My organization is working to make their system more secure. It is my job to ensure the system is safe, investigate all potential security issues, and update employee
computers as needed. The following steps provide examples of how I used SQL with filters to perform security-related tasks.
<br />


<h2>Languages and Utilities Used</h2>

- <b>SQL</b> 



<h2>Program walk-through:</h2>

<h3>Retrieve after hours failed login attempts</h3>
<br />
There was a potential security incident that occurred after business hours (after 18:00). All after hours login attempts that failed need to be investigated.
<br />

The following code demonstrates how I created a SQL query to filter for failed login attempts that occurred after business hours:
<br />

<img src="https://github.com/DRgithubport/Applying-Filters-to-SQL-queries/assets/159063432/b0ffc730-eef7-4731-809f-aaaabb32ca7f"/>
<br />
The first part of the screenshot is my query, and the second part is a portion of the output. This query filters for failed login attempts that occurred after 18:00. First, I started by selecting all data from the log_in_attempts table. Then, I used a WHERE clause with an AND operator to filter my results to output only login attempts that occurred after 18:00 and were unsuccessful. The first condition is login_time > '18:00', which filters for the login
attempts that occurred after 18:00. The second condition is success = FALSE, which filters for the failed login attempts.
<br />
<br />
<h3>Retrieve login attempts on specific dates</h3>
<br/>
A suspicious event occurred on 2022-05-09. Any login activity that happened on 2022-05-09 or on the day before needs to be investigated.
The following code demonstrates how I created a SQL query to filter for login attempts that occurred on specific dates.
<br/>
<br/>

<img src="https://github.com/DRgithubport/Applying-Filters-to-SQL-queries/assets/159063432/749a8929-cd63-4cb5-a49e-94201ee28e46"/>
<br />
The first part of the screenshot is my query, and the second part is a portion of the output. This query returns all login attempts that occurred on 2022-05-09 or 2022-05-08. First, I started by selecting all data from the log_in_attempts table. Then, I used a WHERE clause with an OR operator to filter my results to output only login attempts that occurred on either 2022-05-09 or 2022-05-08. The first condition is login_date = '2022-05-09', which
filters for logins on 2022-05-09. The second condition is login_date = '2022-05-08', which filters for logins on 2022-05-08. <br/>
<br/>
<br/>
<h3>Retrieve login attempts outside of Mexico</h3>
<br/>
After investigating the organization’s data on login a empts, I believe there is an issue with the login a empts that occurred outside of Mexico. These login attempts should be investigated. The following code demonstrates how I created a SQL query to filter for login attempts that occurred outside of Mexico.
<br/>
<br/>
<img src="https://github.com/DRgithubport/Applying-Filters-to-SQL-queries/assets/159063432/f77a6dac-b2d5-46b6-b474-9c062e5f1458"/>
<br />
The first part of the screenshot is my query, and the second part is a portion of the output. This query returns all login attempts that occurred in countries other than Mexico. First, I started by selecting all data from the log_in_attempts table. Then, I used a WHERE clause with NOT to filter for countries other than Mexico. I used LIKE with MEX% as the pattern to match because the dataset represents Mexico as MEX and MEXICO. The percentage sign (%) represents any number of unspecified characters when used with LIKE.
Confirm your selection:  <br/>
<br/>
<br/>
<h3>Retrieve employees in Marketing</h3>
<br/>
My team wants to update the computers for certain employees in the Marketing department. To do this, I have to get information on which employee machines to update. The following code demonstrates how I created a SQL query to  lter for employee machines from employees in the Marketing department in the East building.
<br/>
<br/>
<img src="https://i.imgur.com/cdFHBiU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Wait for process to complete (may take some time):  <br/>
<img src="https://i.imgur.com/JL945Ga.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Sanitization complete:  <br/>
<img src="https://i.imgur.com/K71yaM2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Observe the wiped disk:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
