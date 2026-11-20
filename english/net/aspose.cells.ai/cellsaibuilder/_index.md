---
title: Class CellsAIBuilder
second_title: Aspose.Cells for .NET API Reference
description: "Aspose.Cells.AI.CellsAIBuilder class. Fluent creation of a CellsAI instance. Each builder configures exactly one provider and Build can only succeed once."
type: docs
url: /net/aspose.cells.ai/cellsaibuilder/
---
## CellsAIBuilder class

Fluent creation of a CellsAI instance. Each builder configures exactly one provider and Build can only succeed once.

```csharp
public sealed class CellsAIBuilder
```

## Methods

| Name | Description |
| --- | --- |
| [Build](build/)() | Builds the CellsAI instance, invoking the configured factory exactly once. Resources created by a failed build are cleaned up immediately. |
| [UseAnthropic](useanthropic/)(String, String, Uri) | Configures the Anthropic Messages endpoint. |
| [UseOpenAI](useopenai/)(String, String, Uri) | Configures an OpenAI-compatible chat completion endpoint. |
| [UseOwnedChatClientFactory](useownedchatclientfactory/)(Func<IChatClient>) | Configures a chat client factory that is invoked exactly once during Build. The resulting client is owned by the created CellsAI. |

### See Also

* namespace [Aspose.Cells.AI](../../aspose.cells.ai/)
* assembly [Aspose.Cells.AI](../../)
