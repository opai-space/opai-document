# 🤖 IO Service auto-restart strategy

OPAI Client will automatically detect the working status of IO.NET Worker.&#x20;

When any of the following conditions are met, Launch Binary will be automatically restarted to try to work again.

* No worker containers are running
* Launch container execution exceeds 10 minutes
* Monitor or VC container execution time exceeds 20 minutes, and worker container status is "down" or "unsupported"

