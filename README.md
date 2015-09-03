# ReflectInsight-Listeners-SqlServer

[![Build status](https://ci.appveyor.com/api/projects/status/github/reflectsoftware/reflectinsight-listeners-SqlServer?svg=true)](https://ci.appveyor.com/project/reflectsoftware/reflectinsight-listeners-SqlServer)
[![Release](https://img.shields.io/github/release/reflectsoftware/reflectinsight-listeners-SqlServer.svg)](https://github.com/reflectsoftware/reflectinsight-listeners-SqlServer/releases/latest)
[![NuGet Version](http://img.shields.io/nuget/v/reflectsoftware.insight.listeners.SqlServer.svg?style=flat)](http://www.nuget.org/packages/ReflectSoftware.Insight.Listeners.SqlServer/)
[![NuGet](https://img.shields.io/nuget/dt/reflectsoftware.insight.listeners.SqlServer.svg)](http://www.nuget.org/packages/ReflectSoftware.Insight.Listeners.SqlServer/)
[![Stars](https://img.shields.io/github/stars/reflectsoftware/reflectinsight-listeners-SqlServer.svg)](https://github.com/reflectsoftware/reflectinsight-listeners-SqlServer/stargazers)

## Overview ##

We've added a new destination listener extension for ReflectInsight for logging to SQL Server. This new destination listener extension is called ReflectSoftware.Insight.Listeners.SqlServer and allows you to send logging messages to a SQL Server database.

## Benefits of ReflectInsight Listeners ##

The benefits to using the Insight Listeners is that you can easily and quickly add them to your applicable with little effort and then send ReflectInsight logging messages to other destinations.

## Getting Started

To install ReflectSoftware.Insight.Listeners.SqlServer listener, run the following command in the Package Manager Console:

```powershell
Install-Package ReflectSoftware.Insight.Listeners.SqlServer
```
Then in your app.config or web.config file, add the following configuration sections:

```xml
<?xml version="1.0" encoding="utf-8"?>
<configuration>
  <configSections>        
    <section name="insightSettings" type="ReflectSoftware.Insight.ConfigurationHandler,ReflectSoftware.Insight"/>
  </configSections>
	
  <insightSettings>
    <listeners>

    </listeners>

    

    <listenerGroups active="Active">
      <group name="Active" enabled="true" maskIdentities="false">
        <destinations>
          
        </destinations>
      </group>
    </listenerGroups>
    
    <filters>
      <filter name="ErrorWarningFilter" mode="Include">
        <method type="SendError"/>
        <method type="SendException"/>
        <method type="SendFatal"/>
      </filter>
    </filters>
  </insightSettings>
	
</configuration>
```

Additional configuration details for the ReflectSoftware.Insight.Listeners.SqlServer listener can be found [here](https://reflectsoftware.atlassian.net/wiki/display/RI5/Email+Listener).

## Additional Resources

[Documentation](https://reflectsoftware.atlassian.net/wiki/display/RI5/ReflectInsight+5+documentation)

[Knowledge Base](http://reflectsoftware.uservoice.com/knowledgebase)

[Submit User Feedback](http://reflectsoftware.uservoice.com/forums/158277-reflectinsight-feedback)

[Contact Support](support@reflectsoftware.com)

[ReflectSoftware Website](http://reflectsoftware.com)
