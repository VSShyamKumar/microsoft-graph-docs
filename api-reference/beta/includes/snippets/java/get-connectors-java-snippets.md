---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IConnectorCollectionPage connectors = graphClient.onPremisesPublishingProfiles("applicationProxy").connectors()
	.buildRequest()
	.get();

```