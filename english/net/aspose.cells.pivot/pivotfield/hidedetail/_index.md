---
title: PivotField.HideDetail
second_title: Aspose.Cells for .NET API Reference
description: PivotField method. Sets whether the PivotItems in a pivot field is hidden detail.That is collapse/expand this field
type: docs
url: /net/aspose.cells.pivot/pivotfield/hidedetail/
---
## PivotField.HideDetail method

Sets whether the PivotItems in a pivot field is hidden detail.That is collapse/expand this field.

```csharp
public void HideDetail(bool isHiddenDetail)
```

| Parameter | Type | Description |
| --- | --- | --- |
| isHiddenDetail | Boolean | Whether hide the detail of the pivot field. |

### Examples

```csharp
// Called: pt.RowFields[i].HideDetail(false);
[Test]
        public void Method_Boolean_()
        {
            string filePath = Constants.PivotTableSourcePath + @"JAVA42629_";

            LoadOptions options = new LoadOptions();
            //options.ParsingPivotCachedRecords = true;
            Workbook wb = new Workbook(filePath + "PivotFields.xlsm", options);

            Worksheet ws = wb.Worksheets[0];

            PivotTable pt = ws.PivotTables[0];

            int rowFieldsCount = pt.RowFields.Count;
            for (int i = 0; i < rowFieldsCount; i++)
            {
                //expand PivotField
                pt.RowFields[i].HideDetail(false);
            }


            //you need to comment this code, because the source file doesn't contain the data source of PivotTable, so you can't refresh data.
            //pt.RefreshData();
            pt.CalculateData();

            wb.Save(CreateFolder(filePath) + "out.xlsm");
        }
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


