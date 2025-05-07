---
title: PivotField.IsRepeatItemLabels
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Indicates whether repeating labels of the field in the region. The default value is false
type: docs
url: /net/aspose.cells.pivot/pivotfield/isrepeatitemlabels/
---
## PivotField.IsRepeatItemLabels property

Indicates whether repeating labels of the field in the region. The default value is false.

```csharp
public bool IsRepeatItemLabels { get; set; }
```

### Examples

```csharp
// Called: Assert.IsTrue(workbook.Worksheets["Actual"].PivotTables[0].RowFields[0].IsRepeatItemLabels);
[Test]
        public void Property_IsRepeatItemLabels()
        {


            string filePath = Constants.PivotTableSourcePath + "N43594J41303.xlsx";


            Workbook workbook = new Workbook(filePath);


            Worksheet worksheet = workbook.Worksheets["Actual"];


            PivotTable pivotTable = worksheet.PivotTables[0];


            //Institution field

            pivotTable.RowFields[0].IsRepeatItemLabels = true;

            pivotTable.ColumnFields[0].IsRepeatItemLabels = true;
            workbook.Save(Constants.PivotTableDestPath + "N43594J41303.xlsx");
            workbook = new Workbook(Constants.PivotTableDestPath + "N43594J41303.xlsx");
            Assert.IsTrue(workbook.Worksheets["Actual"].PivotTables[0].RowFields[0].IsRepeatItemLabels);
        }
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


