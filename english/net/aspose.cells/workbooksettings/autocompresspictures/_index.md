---
title: WorkbookSettings.AutoCompressPictures
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. Specifies a boolean value that indicates the application automatically compressed pictures in the workbook
type: docs
url: /net/aspose.cells/workbooksettings/autocompresspictures/
---
## WorkbookSettings.AutoCompressPictures property

Specifies a boolean value that indicates the application automatically compressed pictures in the workbook.

```csharp
public bool AutoCompressPictures { get; set; }
```

### Examples

```csharp
// Called: workbook.Settings.AutoCompressPictures = false;
[Test]
        public void Property_AutoCompressPictures()
        {
            Workbook workbook = new Workbook();
            workbook.Settings.AutoCompressPictures = false;
            workbook.Save(Constants.destPath + "CellsNet41629.xlsx");
            workbook = new Workbook(Constants.destPath + "CellsNet41629.xlsx");
            Assert.AreEqual(workbook.Settings.AutoCompressPictures, false);
        }
```

### See Also

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


