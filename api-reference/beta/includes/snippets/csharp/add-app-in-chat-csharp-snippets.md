---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teamsAppInstallation = new TeamsAppInstallation
{
	AdditionalData = new Dictionary<string, object>()
	{
		{"teamsApp@odata.bind", "https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"}
	}
};

await graphClient.Chats["19:ea28e88c00e94c7786b065394a61f296@thread.v2"].InstalledApps
	.Request()
	.AddAsync(teamsAppInstallation);

```