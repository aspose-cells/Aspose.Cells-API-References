---
title: PivotField.IsAutoSort
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Indicates whether the specified PivotTable field is automatically sorted
type: docs
url: /net/aspose.cells.pivot/pivotfield/isautosort/
---
## PivotField.IsAutoSort property

Indicates whether the specified PivotTable field is automatically sorted.

```csharp
public bool IsAutoSort { get; set; }
```

### Examples

```csharp
// Called: pivotField.IsAutoSort = true;
[Test]
        public void Property_IsAutoSort()
        {
            string filePath = Constants.PivotTableSourcePath + @"NET42556_";

            var book = new Aspose.Cells.Workbook(filePath + "Loss_Ratio_2014-04-12.xls");
            var sheet = book.Worksheets[0];
            var pivot = sheet.PivotTables[0];

            PivotFieldCollection pivotFields = pivot.BaseFields;

            PivotField pivotField = pivotFields["Branch"];

            //Setting the field auto sort
            pivotField.IsAutoSort = true;

            //Setting the field sorting in ascending order
            pivotField.IsAscendSort = true;

            //Sort PivotField named "Branch" via DataField named "GPW"
            pivotField.AutoSortField = 0;

            pivot.CalculateData();
            pivot.RefreshDataOnOpeningFile = true;

            string savePath = CreateFolder(filePath);
            book.Save(savePath + "out.xlsx");
            book.Save(savePath + "out.pdf");

        }
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


