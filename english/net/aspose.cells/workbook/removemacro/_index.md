---
title: Workbook.RemoveMacro
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Removes VBA/macro from this spreadsheet
type: docs
url: /net/aspose.cells/workbook/removemacro/
---
## Workbook.RemoveMacro method

Removes VBA/macro from this spreadsheet.

```csharp
public void RemoveMacro()
```

### Examples

```csharp
// Called: wb.RemoveMacro(); //should not throw Exception
[Test]
        public void Method_RemoveMacro()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;N46854.xlt&quot;);
            wb.RemoveMacro(); //should not throw Exception
        }
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


