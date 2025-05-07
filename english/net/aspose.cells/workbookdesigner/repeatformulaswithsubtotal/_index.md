---
title: WorkbookDesigner.RepeatFormulasWithSubtotal
second_title: Aspose.Cells for .NET API Reference
description: WorkbookDesigner property. Indicates whether repeating formulas with subtotal row
type: docs
url: /net/aspose.cells/workbookdesigner/repeatformulaswithsubtotal/
---
## WorkbookDesigner.RepeatFormulasWithSubtotal property

Indicates whether repeating formulas with subtotal row.

```csharp
public bool RepeatFormulasWithSubtotal { get; set; }
```

### Examples

```csharp
// Called: designer.RepeatFormulasWithSubtotal = (true);//UN-COMMENT THIS LINE TO CHECK THE ISSUE
[Test]
        public void Property_RepeatFormulasWithSubtotal()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "SmartMarker/CellsJava43209.xlsx");
            WorkbookDesigner designer = new WorkbookDesigner(workbook);

            List<Level> list = new List<Level>();
            list.Add(new Level("A", "A1"));
            list.Add(new Level("B", "B1"));
            list.Add(new Level("B", "B2"));
            list.Add(new Level("C", "C1"));
            list.Add(new Level("C", "C2"));
            list.Add(new Level("C", "C3"));

            designer.SetDataSource("Level", list);
            designer.CalculateFormula = (true);
            designer.RepeatFormulasWithSubtotal = (true);//UN-COMMENT THIS LINE TO CHECK THE ISSUE
            designer.Process();

            Assert.AreEqual("=SUBTOTAL(9,E2)", workbook.Worksheets[0].Cells["E3"].Formula);
            //workbook.save(dataDir + "OutPut.xlsx");
            workbook.Save(Constants.destPath + "CellsJava43209.xlsx");
        }
```

### See Also

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


