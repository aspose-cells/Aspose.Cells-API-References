---
title: WorkbookDesigner.Workbook
second_title: Aspose.Cells for .NET API Reference
description: WorkbookDesigner property. Gets and sets the Workbook object
type: docs
url: /net/aspose.cells/workbookdesigner/workbook/
---
## WorkbookDesigner.Workbook property

Gets and sets the `Workbook` object.

```csharp
public Workbook Workbook { get; set; }
```

### Examples

```csharp
// Called: designer.Workbook.Save(Constants.destPath + "Test_121274.xls");
[Test]
        public void Property_Workbook()
        {
           
            WorkbookDesigner designer = new WorkbookDesigner();
            //designer.Open(Constants.sourcePath + "SmartMarker.xls");
            Workbook workbook = new Workbook(Constants.sourcePath + "SmartMarker/SmartMarker.xls");
            designer.Workbook = workbook;
           
            //designer.SetDataSource("Variable", "1");
            //designer.SetDataSource("MultiVariable", new string[] { "1", "Variable 2", "Variable 3" });
            //designer.SetDataSource("MultiVariable2", new string[] { "1", "Skip 2", "Skip 3" });
            DataTable dt = new DataTable();
            dt.Columns.Add("UnitPrice");
            designer.SetDataSource(dt);
            designer.Process(false);

            Assert.IsNull(designer.Workbook.Worksheets[2].Cells["A18"].Value);
            designer.Workbook.Save(Constants.destPath + "Test_121274.xls");
        }
```

### See Also

* class [Workbook](../../workbook/)
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


