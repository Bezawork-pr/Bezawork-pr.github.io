# <pre> Server outage incident report at Company X<img src="https://user-images.githubusercontent.com/107026397/222690413-0b27ca4a-fef3-4daf-89eb-0f5a71f72613.jpg" width=10% height=10%/></pre>
 
<img src="https://user-images.githubusercontent.com/107026397/222704447-0988bfdd-1a8b-492a-83b0-b4e6595c1da8.png" width=3% height=3%/>  Yesterday, on March 2, 2023, at 13:06 PM, we experienced an outage. If you thought you were stressed when you couldn't access your favorite bloggers, imagine Maggie, who not only had to debug the system but also had to deal with our "What Happened Then" fans, who kept calling to know what happens in the next episode. Today, we are providing an incident report detailing what caused the outage and measures taken to minimize future incidents like this.
 
### <pre> Issue Summary </pre>
On Friday, March 2, 2023, at 1:06 PM, our server had an outage until 1:20 PM. The error code response had error code 500. 500 error codes are the worst, aren't they? Followers of bloggers from our company could not access the web pages. The issue affected 100% of the traffic to the server. The root cause of the outage was a typo when including a file with an extension of "phpp instead of php." in the file, wp-setting.php. The lesson we learned is that a simple typo can take a server down.
### <pre> Timeline </pre> 
- 1:06 PM: Changes were made to the file wp-settings.php.
- 1.06 PM: Outage of the server. AKA the happening that server maintainers hope doesn't happen.
- 1:06 PM: Magi was on shift and alerted.
- 1:20 PM: Successful debugging to find the error causing the issue.
- 1:20 PM: Server restarts begin.
- 1:20 PM: 100% of traffic is back online.
 
### <pre> Root cause </pre>
At 1:06 pm, changes were made to the file wp-setting.php. Our team, which works hard to provide you with great services that you enjoy on a daily basis, made a human error. When including another file, a typo in the extension was made, which led to the server responding with error code 500 when users tried to access it.
### <pre> Resolution and recovery </pre>
At 1:06 PM, our team member Magi was alerted. She started debugging right away. Only a few steps were taken to find the bug, as it was not a complicated system failure. She started debugging to find what was causing the error, and in two steps she was able to find the root cause of the error. She put debugging on wp-config.php, which resolved the 500 error code. Though the 500 error code was resolved, the server was still returning an empty string. Then she used the curl command with flag -4 to get details of what was happening. This command returned a file trying to be included that could not be found and saw that it has a typo in the extension; this was resolved by editing the file.
### <pre> Corrective and preventative measures </pre>
This morning, we conducted an internal review of the outage. Everyone is pointing fingers at Harold. JK, we are blame-free postmortem. We discussed how we can reduce such issues in the future. And have come to the common conclusion that the following steps should be taken:

- For now, add one more server and more as the traffic grows.
- Peer reviews come before changes.
 
Sincerely,

The X company








