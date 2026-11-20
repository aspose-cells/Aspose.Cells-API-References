---
title: CellsAIBuilder.UseOwnedChatClientFactory
second_title: Aspose.Cells for .NET API Reference
description: "CellsAIBuilder method. Configures a chat client factory that is invoked exactly once during Build. The resulting client is owned by the created CellsAI."
type: docs
url: /net/aspose.cells.ai/cellsaibuilder/useownedchatclientfactory/
---
## CellsAIBuilder.UseOwnedChatClientFactory method

Configures a chat client factory that is invoked exactly once during Build. The resulting client is owned by the created CellsAI.

```csharp
public CellsAIBuilder UseOwnedChatClientFactory(Func<IChatClient> chatClientFactory)
```

| Parameter | Type | Description |
| --- | --- | --- |
| chatClientFactory | Func<IChatClient> | The factory that creates the chat client owned by the new Cells AI instance. |

### Return Value

A CellsAIBuilder.

### See Also

* class [CellsAIBuilder](../)
* namespace [Aspose.Cells.AI](../../../aspose.cells.ai/)
* assembly [Aspose.Cells.AI](../../../)
