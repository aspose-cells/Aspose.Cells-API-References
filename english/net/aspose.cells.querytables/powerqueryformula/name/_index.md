---
title: PowerQueryFormula.Name
second_title: Aspose.Cells for .NET API Reference
description: PowerQueryFormula property. Gets and sets the name of the power query formula
type: docs
url: /net/aspose.cells.querytables/powerqueryformula/name/
---
## PowerQueryFormula.Name property

Gets and sets the name of the power query formula.

```csharp
public string Name { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual("tPeriodTable", mashupData.PowerQueryFormulas[2].Name);
[Test]
        public void Property_Name()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet47494.xlsm");

            DataMashup mashupData = workbook.DataMashup;
            
            Assert.AreEqual("Timesheets", mashupData.PowerQueryFormulas[0].Name);
            Assert.AreEqual("PQVLookUp", mashupData.PowerQueryFormulas[1].Name);
            Assert.AreEqual("tPeriodTable", mashupData.PowerQueryFormulas[2].Name);
            workbook.Save(Constants.destPath + "CellsNet47494.xlsm");

            workbook = new Workbook(Constants.sourcePath + "CellsNet47494.xlsx");

            mashupData = workbook.DataMashup;
            foreach (PowerQueryFormula f in mashupData.PowerQueryFormulas)
            {
                Console.WriteLine(f.Name);
            }
            workbook.Save(Constants.destPath + "CellsNet47494.xlsx");
        }
```

### See Also

* class [PowerQueryFormula](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


