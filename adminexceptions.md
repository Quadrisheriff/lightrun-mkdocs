---
id: adminexceptions
title: Configure and monitor exceptions
---
Lightrun has the ability to monitor all the exceptions thrown in the
application and give insights about them.

**Note:** By default, every exception in the application will be
reported, even ones that get caught along the way.

Configuring the Agent {#_configuring_the_agent}
---------------------

In order to configure the agent to report the exceptions to the server
follow these steps:

1.  Go to the folder of the agent

2.  Open the `agent.config` file

3.  Find the property `exceptions_monitoring_enabled` and set it to `1`.
    It should look like this: `exceptions_monitoring_enabled=1`

4.  In case you want the agent to ignore exceptions that are caught
    along the way, find and set the `exceptions_should_report_caught`
    property to `0`.

5.  Restart your application with the agent

The Server {#_the_server}
----------

In the server you'll be able to see general statistics about the
exceptions and details of specific exceptions. To view the exceptions
table, click Exceptions → Data

![Exceptions Menu](../../img/exceptions-menu.png)

In this page you'll be able to see a table with statistics on all the
exceptions thrown by all your applications.

![Exceptions Table](../../img/exceptions-table.png)

In the top right corner of the screen there are search options. You can
search with free text and by specific time frames or by custom range.

![Exceptions Search](../../img/exceptions-search.png)

Clicking on a specific type of exception in the table will open a modal
with more details on the exception. Clicking on a specific exception in
the table (or navigating using the \"Previous/Next Exception\" buttons
above) you'll be able to see the stacktrace of each specific exception,
and for each frame in the stacktrace you can see the snapshot of the
frame.

![Exceptions Details](../../img/exceptions-details.png)


