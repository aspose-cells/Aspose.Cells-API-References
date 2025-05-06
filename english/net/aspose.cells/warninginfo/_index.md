---
title: Class WarningInfo
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.WarningInfo class. Warning info
type: docs
url: /net/aspose.cells/warninginfo/
---
## WarningInfo class

Warning info

```csharp
public class WarningInfo
```

## Properties

| Name | Description |
| --- | --- |
| [CorrectedObject](../../aspose.cells/warninginfo/correctedobject/) { get; set; } | Gets and sets the corrected object. |
| [Description](../../aspose.cells/warninginfo/description/) { get; } | Get description of warning info. |
| [ErrorObject](../../aspose.cells/warninginfo/errorobject/) { get; } | The error object. |
| [Type](../../aspose.cells/warninginfo/type/) { get; } | Get warning type. |
| [WarningType](../../aspose.cells/warninginfo/warningtype/) { get; } | (**Obsolete.**) Get warning type. |

### Examples

```csharp
// Called: public void Warning(WarningInfo warningInfo)
public void Type_WarningInfo(WarningInfo warningInfo)
            {
                Assert.AreEqual(warningInfo.Type, ExceptionType.DefinedName);
                Assert.IsTrue(warningInfo.Description.StartsWith(&quot;Duplicate defined name: _XLNM.PRINT_AREA;ReferTo:&quot;));
            }
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


