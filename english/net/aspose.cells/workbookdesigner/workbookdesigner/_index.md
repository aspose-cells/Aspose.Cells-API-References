---
title: WorkbookDesigner.WorkbookDesigner
second_title: Aspose.Cells for .NET API Reference
description: WorkbookDesigner constructor. Initializes a new instance of the WorkbookDesigner class
type: docs
url: /net/aspose.cells/workbookdesigner/workbookdesigner/
---
## WorkbookDesigner() {#constructor}

Initializes a new instance of the [`WorkbookDesigner`](../) class.

```csharp
public WorkbookDesigner()
```

### Examples

```csharp
// Called: designer = new WorkbookDesigner();
[Test]
        public void WorkbookDesigner_Constructor()
        {
            string dirPath = Constants.sourcePath + "SmartMarker/CellsNet43432";

            Workbook workbook;
            WorkbookDesigner designer;
            DataSet ds = new DataSet();

            ds.ReadXmlSchema(dirPath + "/schema.xml");
            ds.ReadXml(dirPath + "/data.xml");

            workbook = new Workbook(dirPath + "/Template.xls");
            designer = new WorkbookDesigner();
            designer.Workbook = workbook;
            designer.SetDataSource(ds);
            designer.Process(true);

            Assert.AreEqual(true,workbook.Worksheets["Skip"].Cells["B27"].IsFormula);

        }
```

### See Also

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## WorkbookDesigner(Workbook) {#constructor_1}

Initializes a new instance of the [`WorkbookDesigner`](../) class.

```csharp
public WorkbookDesigner(Workbook workbook)
```

| Parameter | Type | Description |
| --- | --- | --- |
| workbook | Workbook | The template workbook file. |

### Examples

```csharp
// Called: var designer = new WorkbookDesigner(wb);
[Test]
        public void WorkbookDesigner_Constructor()
        {
            Workbook wb = new Workbook();
            var sheet = wb.Worksheets[0];
            //create 2x1 merge cell
            sheet.Cells.CreateRange(0, 0, 1, 2).Merge();
            sheet.Cells[0, 0].Value = "&=obj.Property(group:merge)";
            sheet.Cells[0, 2].Value = "&=obj.AABB";
            //output template file
            const string templateFile = "template.xlsx";
            //    wb.Save(templateFile);
            //   Process.Start("cmd", $"/c start {templateFile}");
            var designer = new WorkbookDesigner(wb);
            designer.SetDataSource("obj", new[] { new objClass("Value1", "Value2"), new objClass("Value1", "Value2"), new objClass("Value1", "Value3"), new objClass("Value1", "Value4"), new objClass("Value2", "Value2") });
            designer.Process();
            CellArea ca = (CellArea)wb.Worksheets[0].Cells.GetMergedAreas()[0];
            Assert.AreEqual(3, ca.EndRow);

            wb.Save(Constants.destPath + "CellsNet52236.xlsx");
        }
```

### See Also

* class [Workbook](../../workbook/)
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


