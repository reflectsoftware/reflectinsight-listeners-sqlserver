﻿# Hello ReflectInsight Sample

This sample will show you how to start working with ReflectInsight with no configuration and the results will show up in the ReflectInsight Live Viewer.

## Getting Started

1. To install ReflectInsight, run the following command in the Package Manager Console:

	```powershell
	Install-Package ReflectSoftware.Insight
	```

2. Next add a using reference to the ReflectSofteare.Insight namespace.

	```csharp
	using ReflectSoftware.Insight;
	```

3. Then for this sample we're going to use the default log manager for sending our log message.

	```csharp
	RILogManager.Default.SendMessage("Hello, ReflectInsight!");
	```

4. That's it your done! Build your app and check it out.


## Resources

Please refer to the ReflectInsight [Documentation](https://reflectsoftware.atlassian.net/wiki/display/RI5/ReflectInsight+5+documentation) for details on configuring ReflectInsight.
       
Feedback is always welcome on our [UserVoice](http://reflectsoftware.uservoice.com/forums/158277-reflectinsight-feedback).

Contact [support](support@reflectsoftware.com) for any help!