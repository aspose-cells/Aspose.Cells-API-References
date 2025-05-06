---
title: Workbook.RemovePersonalInformation
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Removes personal information
type: docs
url: /net/aspose.cells/workbook/removepersonalinformation/
---
## Workbook.RemovePersonalInformation method

Removes personal information.

```csharp
public void RemovePersonalInformation()
```

### Examples

```csharp
// Called: wb.RemovePersonalInformation();
[Test]
        public void Method_RemovePersonalInformation()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;CellsNet47877.xlsx&quot;);
            Assert.IsTrue(wb.Settings.RemovePersonalInformation);
            wb.RemovePersonalInformation();
            // Save the Excel file.
            wb.Save(Constants.destPath + &quot;CellsNet47877.xlsx&quot;, SaveFormat.Xlsx);
            wb = new Workbook(Constants.destPath + &quot;CellsNet47877.xlsx&quot;);
            Assert.IsTrue(wb.Worksheets[0].Comments[1].Note.Contains(&quot;Author&quot;));
        }
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


