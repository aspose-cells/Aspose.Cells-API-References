---
title: WorkbookSettings.UpdateLinksType
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. Gets and sets how updates external links when the workbook is opened
type: docs
url: /net/aspose.cells/workbooksettings/updatelinkstype/
---
## WorkbookSettings.UpdateLinksType property

Gets and sets how updates external links when the workbook is opened.

```csharp
public UpdateLinksType UpdateLinksType { get; set; }
```

### Examples

```csharp
// Called: workbook.Settings.UpdateLinksType = UpdateLinksType.Never;
[Test]
        public void Property_UpdateLinksType()
        {
            Workbook workbook = new Workbook();
            workbook.Settings.UpdateLinksType = UpdateLinksType.Never;
            workbook.Save(Constants.destPath + "CELLSJAVA41007.xlsx");
            workbook = new Workbook(Constants.destPath + "CELLSJAVA41007.xlsx");
            Assert.AreEqual(workbook.Settings.UpdateLinksType, UpdateLinksType.Never);

        }
```

### See Also

* enum [UpdateLinksType](../../updatelinkstype/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


