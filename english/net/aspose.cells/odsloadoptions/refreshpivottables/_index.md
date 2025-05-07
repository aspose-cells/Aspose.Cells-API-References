---
title: OdsLoadOptions.RefreshPivotTables
second_title: Aspose.Cells for .NET API Reference
description: OdsLoadOptions property. Indicates whether refresh pivot tables when loading file
type: docs
url: /net/aspose.cells/odsloadoptions/refreshpivottables/
---
## OdsLoadOptions.RefreshPivotTables property

Indicates whether refresh pivot tables when loading file.

```csharp
public bool RefreshPivotTables { get; set; }
```

### Examples

```csharp
// Called: loadOptions.RefreshPivotTables = true;
[Test]
        public void Property_RefreshPivotTables()
        {
            Workbook wb = new Workbook(Constants.sourcePath + "CellsNet45916.xlsx");

            wb.Save(Constants.destPath + "CellsNet45916.ods");
            OdsLoadOptions loadOptions = new OdsLoadOptions();
            loadOptions.RefreshPivotTables = true;
            wb = new Workbook(Constants.destPath + "CellsNet45916.ods", loadOptions);
            wb.Save(Constants.destPath + "CellsNet45916.html");
            Cell cell = wb.Worksheets[0].Cells["L20"];
            Assert.AreEqual("Sports Type", cell.StringValue);
        }
```

### See Also

* class [OdsLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


