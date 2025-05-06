---
title: WorkbookDesigner.CalculateFormula
second_title: Aspose.Cells for .NET API Reference
description: WorkbookDesigner property. Indicates whether formulas should be calculated
type: docs
url: /net/aspose.cells/workbookdesigner/calculateformula/
---
## WorkbookDesigner.CalculateFormula property

Indicates whether formulas should be calculated.

```csharp
public bool CalculateFormula { get; set; }
```

### Examples

```csharp
// Called: designer.CalculateFormula = true;
[Test]
        public void Property_CalculateFormula()
        {
            DataSet dataSet = new DataSet();


            string DIR = Constants.sourcePath + &quot;SmartMarker/CellsNet42958/&quot;;


            // Gather a list of the files in the Data directory

            dataSet.ReadXmlSchema(DIR + &quot;/Data/schema.xml&quot;);

            dataSet.ReadXml(DIR + &quot;/Data/data.xml&quot;);


            DataSet ds = dataSet;


            Workbook workbook = new Workbook(DIR + &quot;/Data/excel_before_merge.xlsx&quot;);

            WorkbookDesigner designer = new WorkbookDesigner(workbook);

            designer.SetDataSource(ds);

            designer.CalculateFormula = true;

            designer.Process(false);


            Assert.AreEqual(workbook.Worksheets[0].Cells[&quot;J10&quot;].IsFormula, true);
        }
```

### See Also

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


