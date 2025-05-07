---
title: Protection.AllowEditingObject
second_title: Aspose.Cells for .NET API Reference
description: Protection property. Represents if the user is allowed to manipulate drawing objects on a protected worksheet
type: docs
url: /net/aspose.cells/protection/alloweditingobject/
---
## Protection.AllowEditingObject property

Represents if the user is allowed to manipulate drawing objects on a protected worksheet.

```csharp
public bool AllowEditingObject { get; set; }
```

### Examples

```csharp
// Called: Assert.IsFalse(sheet.Protection.AllowEditingObject);
[Test]
        public void Property_AllowEditingObject()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet45687.xml");
            Worksheet sheet = workbook.Worksheets[0];
            Assert.IsFalse(sheet.Protection.AllowEditingScenario);
            Assert.IsFalse(sheet.Protection.AllowEditingObject);
            workbook.Save(Constants.destPath + "CellsNet45687.xml");
            workbook = new Workbook(Constants.destPath + "CellsNet45687.xml");
            Assert.IsFalse(sheet.Protection.AllowEditingScenario);
            Assert.IsFalse(sheet.Protection.AllowEditingObject);
            workbook.Save(Constants.destPath + "CellsNet45687.xml");
        }
```

### See Also

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


