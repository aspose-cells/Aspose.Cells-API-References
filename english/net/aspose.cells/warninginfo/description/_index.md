---
title: WarningInfo.Description
second_title: Aspose.Cells for .NET API Reference
description: WarningInfo property. Get description of warning info
type: docs
url: /net/aspose.cells/warninginfo/description/
---
## WarningInfo.Description property

Get description of warning info.

```csharp
public string Description { get; }
```

### Examples

```csharp
// Called: Assert.IsTrue(warningInfo.Description.StartsWith("Duplicate defined name: _XLNM.PRINT_AREA;ReferTo:"));
public void WarningInfo_Property_Description(WarningInfo warningInfo)
            {
                Assert.AreEqual(warningInfo.Type, ExceptionType.DefinedName);
                Assert.IsTrue(warningInfo.Description.StartsWith("Duplicate defined name: _XLNM.PRINT_AREA;ReferTo:"));
            }
```

### See Also

* class [WarningInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


