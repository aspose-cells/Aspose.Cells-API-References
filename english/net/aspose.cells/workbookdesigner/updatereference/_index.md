---
title: WorkbookDesigner.UpdateReference
second_title: Aspose.Cells for .NET API Reference
description: WorkbookDesigner property. Indicates if references in other worksheets will be updated
type: docs
url: /net/aspose.cells/workbookdesigner/updatereference/
---
## WorkbookDesigner.UpdateReference property

Indicates if references in other worksheets will be updated.

```csharp
public bool UpdateReference { get; set; }
```

### Examples

```csharp
// Called: designer.UpdateReference = true;
[Test]
        public void Property_UpdateReference()
        {
            string filePath = Constants.PivotTableSourcePath + @"NET46883_";

            DataSet ds = new DataSet();
            ds.ReadXml(filePath + "EQDCV.RAW.XML");
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.UpdateReference = true;
            designer.UpdateEmptyStringAsNull = true;
            designer.Workbook = new Workbook(filePath + "EQDCV.XLSX");
            designer.SetDataSource("RAW", new DataView(ds.Tables[0]));
            designer.Process();
            foreach (Worksheet worksheet in designer.Workbook.Worksheets)
            {
                worksheet.RefreshPivotTables();
            }
            designer.Workbook.Save(CreateFolder(filePath) + "out.xlsx");
        }
```

### See Also

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


