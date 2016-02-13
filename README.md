# spring_boot_project
Spring boot startup application

This is the Spring boot startup "Hello World!" application. 

Tips:-
When you run the application, if you get java.net.BindException: Address already in use: bind.

In windows, you can run the below commands to resolve the issue.

c:\>netstat -ano | find "8080"
TCP    0.0.0.0:8080           0.0.0.0:0              LISTENING       1196
TCP    [::]:8080              [::]:0                 LISTENING       1196
c:\>taskkill /F /PID 1196
SUCCESS: The process with PID 1196 has been terminated.
