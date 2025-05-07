---
title: PivotField.ShowSubtotalAtTop
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. when ShowInOutlineForm is true then display subtotals at the top of the list of items instead of at the bottom
type: docs
url: /net/aspose.cells.pivot/pivotfield/showsubtotalattop/
---
## PivotField.ShowSubtotalAtTop property

when ShowInOutlineForm is true, then display subtotals at the top of the list of items instead of at the bottom

```csharp
public bool ShowSubtotalAtTop { get; set; }
```

### Remarks

Only works when ShowInOutlineForm is true.

### Examples

```csharp
// Called: f.ShowSubtotalAtTop = true;
[Test]
        public void Property_ShowSubtotalAtTop()
        {
            string filePath = Constants.PivotTableSourcePath + @"NET43877_";
            LoadOptions loadOptions = new LoadOptions();
            Workbook workbook = new Workbook(filePath + "Customer.xlsx", loadOptions);
            Worksheet sheet2 = workbook.Worksheets[workbook.Worksheets.Add()];
            sheet2.Name = "Summary";
            Aspose.Cells.Pivot.PivotTableCollection pivotTables = sheet2.PivotTables;

            //int index = pivotTables.Add("=" + workbook.Worksheets[0].Name + "!A1:Y" + workbook.Worksheets[0].Cells.MaxDataRow + 1, "B3", "PivotTable1");
            int index = pivotTables.Add("=" + workbook.Worksheets[0].Name + "!A1:Y" + (workbook.Worksheets[0].Cells.MaxDataRow + 1), "B3", "PivotTable1");

            Console.WriteLine("=" + workbook.Worksheets[0].Name + "!A1:Y" + workbook.Worksheets[0].Cells.MaxDataRow + 1);
            Console.WriteLine("=" + workbook.Worksheets[0].Name + "!A1:Y" + (workbook.Worksheets[0].Cells.MaxDataRow + 1));
            //Accessing the instance of the newly added PivotTable 

            Aspose.Cells.Pivot.PivotTable pivotTable = pivotTables[index];

            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, "AU No");
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, "Debtor/Search Name");
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, "Obligor No");
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, "Date/Time");
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, "Fee");

            if (pivotTable.DataField != null)
            {
                //DataField attribute of PivotTable exists only if DataFields contains two or more PivotField 
                pivotTable.AddFieldToArea(PivotFieldType.Column, pivotTable.DataField);
            }

            //add for layout
            int rowFieldsCount = pivotTable.RowFields.Count;
            for (int j = 0; j < rowFieldsCount; j++)
            {
                PivotField f = pivotTable.RowFields[j];
                f.ShowCompact = true;
                f.ShowInOutlineForm = true;
                f.ShowSubtotalAtTop = true;
            }
            pivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium9;
            //end

            workbook.Save(Constants.PIVOT_CHECK_FILE_PATH + "NET43877.xlsx");
        }
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


