---
title: Protection.AllowFiltering
second_title: Aspose.Cells for .NET API Reference
description: Protection property. Represents if the user is allowed to make use of an AutoFilter that was created before the sheet was protected
type: docs
url: /net/aspose.cells/protection/allowfiltering/
---
## Protection.AllowFiltering property

Represents if the user is allowed to make use of an AutoFilter that was created before the sheet was protected.

```csharp
public bool AllowFiltering { get; set; }
```

### Examples

```csharp
// Called: Assert.IsTrue(workbook.Worksheets[0].Protection.AllowFiltering);
[Test]
        public void Property_AllowFiltering()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet45548.xml&quot;);
            Assert.IsTrue(workbook.Worksheets[0].Protection.AllowFiltering);
            workbook.Save(Constants.destPath + &quot;CellsNet45548.xml&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CellsNet45548.xml&quot;);
            Assert.IsTrue(workbook.Worksheets[0].Protection.AllowFiltering);
        }
```

### See Also

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


