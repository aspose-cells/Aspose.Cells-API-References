---
title: WorkbookDesigner.SetJsonDataSource
second_title: Aspose.Cells for .NET API Reference
description: WorkbookDesigner method. 
type: docs
url: /net/aspose.cells/workbookdesigner/setjsondatasource/
---
## WorkbookDesigner.SetJsonDataSource method

```csharp
public void SetJsonDataSource(string variable, string data)
```

| Parameter | Type | Description |
| --- | --- | --- |
| variable | String |  |
| data | String |  |

### Examples

```csharp
// Called: designer.SetJsonDataSource("node", jsonFile);
[Test]
        public void Method_String_()
        {
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.Workbook = (new Workbook(Constants.sourcePath + "CELLSJAVA46326_smart_markers.xlsx"));
           // designer.Workbook.Worksheets[0].Cells.SetRowHeightPixel(1, 17);
            String jsonFile = File.ReadAllText(Constants.sourcePath + "CELLSJAVA46326_smartMarkers.json");
            designer.SetJsonDataSource("node", jsonFile);
            designer.Process();
          
            foreach (Worksheet sheet in designer.Workbook.Worksheets)
            {
                sheet.AutoFitRows();
            }
            Assert.AreEqual(225, designer.Workbook.Worksheets[0].Shapes[0].Height);
            designer.Workbook.Save(Constants.destPath + "CELLSJAVA46326.xlsx");
        }
```

### See Also

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


