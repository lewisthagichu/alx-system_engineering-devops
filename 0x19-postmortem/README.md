## Incident Summary

**Outage Duration**

The service disruption occurred from 15:00 to 17:00 local time.

**Impact**

The primary service, responsible for processing incoming requests, experienced sluggish performance, leading to delays in addressing user requests. Approximately 30% of users were affected.

**Root Cause**

A critical bug within the code triggered a memory leak, depleting available resources and causing a slowdown in service operations.

**Timeline**

- 15:15:
  The issue was identified through performance monitoring.

- 15:30:
  Engineers initiated an investigation, initially suspecting a potential server load issue.

- 16:00:
  Examination of logs and performance metrics revealed a memory leak as the culprit for the slowdown.

- 16:15:
  The problem was reported to the development team for further analysis and resolution.

- 17:05:
  Developers successfully identified and rectified the root cause, restoring the service to normal functionality.

**Root Cause and Solution**

The underlying problem stemmed from a code-related memory leak. The solution involved addressing and rectifying the coding error, coupled with resource optimization measures.

For a visual representation, please refer to the attached diagram illustrating the incident timeline and resolution process.
![alt text](https://raw.githubusercontent.com/lewisthagichu/alx-system_engineering-devops/master/0x19-postmortem/assets/1.webp?raw=true)  
The figure belowshows how to resolve plus how the error occured
![alt text](https://raw.githubusercontent.com/lewisthagichu/alx-system_engineering-devops/master/0x19-postmortem/assets/2.webp?raw=true)  

