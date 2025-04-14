---
title: Class AbstractLowCodeSaveOptionsProvider
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.LowCode.AbstractLowCodeSaveOptionsProvider class. Implementation to provide multiple save options for processes that require multiple outputs. For example SpreadsheetSplitter feature requires multiple destinations to save the split files
type: docs
url: /net/aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/
---
## AbstractLowCodeSaveOptionsProvider class

Implementation to provide multiple save options for processes that require multiple outputs. For example, [`SpreadsheetSplitter`](../spreadsheetsplitter/) feature requires multiple destinations to save the split files.

```csharp
public abstract class AbstractLowCodeSaveOptionsProvider
```

## Methods

| Name | Description |
| --- | --- |
| virtual [Finish](../../aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/finish/)(LowCodeSaveOptions) | Releases resources after processing currently split part. |
| abstract [GetSaveOptions](../../aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/getsaveoptions/)(SplitPartInfo) | Gets the save options from which to get the output settings for currently split part. Returning null denotes to skip given part. |

### See Also

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


