The SharePoint Framework contains a logging API that can be used to log messages during the lifecycle of your webpart. The API documentation is here - https://sharepoint.github.io/classes/_sp_client_base_.log.html
The logging levels are fairly standard, with Verbose being the least important, followed by Info, Warning and Error.
Here is how you go about using it.
Reference the Log class:  
import{ Log } from '@microsoft/sp-core-library'; 
Log your message from your WebPart:
Log.verbose("HelloWorld", "Here is a verbose log", this.context.serviceScope);
Log.info("HelloWorld", "Here is an informational message.", this.context.serviceScope);
Log.warn("HelloWorld", "Oh Oh, this might be bad", this.context.serviceScope);
Log.error("HelloWorld", new Error("Oh No!  Error!  Ahhhhhh!!!!"), this.context.serviceScope);
This will result in the following in the debug console

MS will be adding features around logging in the future.


https://github.com/SharePoint/sp-dev-docs/wiki/Working-with-the-Logging-API