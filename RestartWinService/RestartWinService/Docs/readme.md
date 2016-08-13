# Chamindac.vsts.release.task.restart-win-service

Release task that enable you to restart windows service with all the dependant services.

![Restart Win Service](https://chamindac.gallery.vsassets.io/_apis/public/gallery/publisher/chamindac/extension/chamindac-vsts-release-task-restart-win-service/1.0.5/privateasset/eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJwbiI6ImNoYW1pbmRhYyIsImVuIjoiY2hhbWluZGFjLXZzdHMtcmVsZWFzZS10YXNrLXJlc3RhcnQtd2luLXNlcnZpY2UiLCJleHAiOiIxNDcxNzE2OTk1In0=.RE9xSHkrSUZSbEUrTWczRlYrZ3U5TnZldW4rWGcrS0kzM09aczNRWUR4RT0=/Microsoft.VisualStudio.Services.Screenshots.1)

Task requires one mandatory parameter Service Name. For this parameter Service Name or Service Display name can be provided.

![Restart Win Service](https://chamindac.gallery.vsassets.io/_apis/public/gallery/publisher/chamindac/extension/chamindac-vsts-release-task-restart-win-service/1.0.5/privateasset/eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJwbiI6ImNoYW1pbmRhYyIsImVuIjoiY2hhbWluZGFjLXZzdHMtcmVsZWFzZS10YXNrLXJlc3RhcnQtd2luLXNlcnZpY2UiLCJleHAiOiIxNDcxNzE2OTk1In0=.RE9xSHkrSUZSbEUrTWczRlYrZ3U5TnZldW4rWGcrS0kzM09aczNRWUR4RT0=/Microsoft.VisualStudio.Services.Screenshots.2)

Once run it will stop all dependent services that are running currently, and restart the main service, then start the dependent services stopped earlier. The dependent services that were not running when the restart request made, will not be started, so that the system services state will remain same after restart service script run.

![Restart Win Service](https://chamindac.gallery.vsassets.io/_apis/public/gallery/publisher/chamindac/extension/chamindac-vsts-release-task-restart-win-service/1.0.5/privateasset/eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJwbiI6ImNoYW1pbmRhYyIsImVuIjoiY2hhbWluZGFjLXZzdHMtcmVsZWFzZS10YXNrLXJlc3RhcnQtd2luLXNlcnZpY2UiLCJleHAiOiIxNDcxNzE2OTk1In0=.RE9xSHkrSUZSbEUrTWczRlYrZ3U5TnZldW4rWGcrS0kzM09aczNRWUR4RT0=/Microsoft.VisualStudio.Services.Screenshots.3)

# Documentation

Please check the [Get started](http://chamindac.blogspot.com/2016/08/restart-widows-servicesvststfs-release.html)

# Known Issues

If release agent is running with user such as NetworService, error could occur. 

For example restarting w3svc could fail with "Service 'World Wide Web Publishing Service (w3svc)' cannot be stopped due to the following error: Cannot open w3svc service on computer '.'".
)