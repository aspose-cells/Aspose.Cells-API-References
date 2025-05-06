---
title: Protection.AllowEditingScenario
second_title: Aspose.Cells for .NET API Reference
description: Protection property. Represents if the user is allowed to edit scenarios on a protected worksheet
type: docs
url: /net/aspose.cells/protection/alloweditingscenario/
---
## Protection.AllowEditingScenario property

Represents if the user is allowed to edit scenarios on a protected worksheet.

```csharp
public bool AllowEditingScenario { get; set; }
```

### Examples

```csharp
// Called: Assert.IsFalse(sheet.Protection.AllowEditingScenario);
[Test]
        public void Property_AllowEditingScenario()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet45687.xml&quot;);
            Worksheet sheet = workbook.Worksheets[0];
            Assert.IsFalse(sheet.Protection.AllowEditingScenario);
            Assert.IsFalse(sheet.Protection.AllowEditingObject);
            workbook.Save(Constants.destPath + &quot;CellsNet45687.xml&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CellsNet45687.xml&quot;);
            Assert.IsFalse(sheet.Protection.AllowEditingScenario);
            Assert.IsFalse(sheet.Protection.AllowEditingObject);
            workbook.Save(Constants.destPath + &quot;CellsNet45687.xml&quot;);
        }
```

### See Also

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


