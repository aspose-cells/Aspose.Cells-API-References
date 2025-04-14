---
title: Class AbstractLowCodeLoadOptionsProvider
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.LowCode.AbstractLowCodeLoadOptionsProvider class. Implementation to provide multiple load options for processes that use multiple inputssuch as template files
type: docs
url: /net/aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/
---
## AbstractLowCodeLoadOptionsProvider class

Implementation to provide multiple load options for processes that use multiple inputs(such as template files).

```csharp
public abstract class AbstractLowCodeLoadOptionsProvider
```

## Properties

| Name | Description |
| --- | --- |
| abstract [Current](../../aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/current/) { get; } | Gets the load options from which to load data of currently processed part. |

## Methods

| Name | Description |
| --- | --- |
| virtual [Finish](../../aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/finish/)(LowCodeLoadOptions) | Releases resources after processing currently part of input. |
| abstract [MoveNext](../../aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/movenext/)() | Checks whether there is more input. |

### Remarks

For example, [`SpreadsheetMerger`](../spreadsheetmerger/) feature requires multiple template files to merge.

### See Also

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


