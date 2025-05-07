---
title: Protection.AllowEditingContent
second_title: Aspose.Cells for .NET API Reference
description: Protection property. Represents if the user is allowed to edit contents of locked cells on a protected worksheet
type: docs
url: /net/aspose.cells/protection/alloweditingcontent/
---
## Protection.AllowEditingContent property

Represents if the user is allowed to edit contents of locked cells on a protected worksheet.

```csharp
public bool AllowEditingContent { get; set; }
```

### Examples

```csharp
// Called: Assert.IsTrue(!workbook.Worksheets["Graph"].Protection.AllowEditingContent);
[Test]
        public void Property_AllowEditingContent()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET56881.xlsb");
            workbook.Save(Constants.destPath + "CELLSNET56881.xlsx");
            workbook = new Workbook(Constants.destPath + "CELLSNET56881.xlsx");
            Assert.IsTrue(!workbook.Worksheets["Graph"].Protection.AllowEditingContent);
            workbook.Save(Constants.destPath + "CELLSNET56881.xlsb");
            workbook = new Workbook(Constants.destPath + "CELLSNET56881.xlsb");
            Assert.IsTrue(!workbook.Worksheets["Graph"].Protection.AllowEditingContent);

        }
```

### See Also

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


