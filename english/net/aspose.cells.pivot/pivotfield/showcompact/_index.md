---
title: PivotField.ShowCompact
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Indicates whether display labels from the next field in the same column on the Pivot Table view
type: docs
url: /net/aspose.cells.pivot/pivotfield/showcompact/
---
## PivotField.ShowCompact property

Indicates whether display labels from the next field in the same column on the Pivot Table view

```csharp
public bool ShowCompact { get; set; }
```

### Examples

```csharp
// Called: f.ShowCompact = true;
[Test]
        public void Property_ShowCompact()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;NET43877_&quot;;
            LoadOptions loadOptions = new LoadOptions();
            Workbook workbook = new Workbook(filePath + &quot;Customer.xlsx&quot;, loadOptions);
            Worksheet sheet2 = workbook.Worksheets[workbook.Worksheets.Add()];
            sheet2.Name = &quot;Summary&quot;;
            Aspose.Cells.Pivot.PivotTableCollection pivotTables = sheet2.PivotTables;

            //int index = pivotTables.Add(&quot;=&quot; + workbook.Worksheets[0].Name + &quot;!A1:Y&quot; + workbook.Worksheets[0].Cells.MaxDataRow + 1, &quot;B3&quot;, &quot;PivotTable1&quot;);
            int index = pivotTables.Add(&quot;=&quot; + workbook.Worksheets[0].Name + &quot;!A1:Y&quot; + (workbook.Worksheets[0].Cells.MaxDataRow + 1), &quot;B3&quot;, &quot;PivotTable1&quot;);

            Console.WriteLine(&quot;=&quot; + workbook.Worksheets[0].Name + &quot;!A1:Y&quot; + workbook.Worksheets[0].Cells.MaxDataRow + 1);
            Console.WriteLine(&quot;=&quot; + workbook.Worksheets[0].Name + &quot;!A1:Y&quot; + (workbook.Worksheets[0].Cells.MaxDataRow + 1));
            //Accessing the instance of the newly added PivotTable 

            Aspose.Cells.Pivot.PivotTable pivotTable = pivotTables[index];

            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, &quot;AU No&quot;);
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, &quot;Debtor/Search Name&quot;);
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, &quot;Obligor No&quot;);
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, &quot;Date/Time&quot;);
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, &quot;Fee&quot;);

            if (pivotTable.DataField != null)
            {
                //DataField attribute of PivotTable exists only if DataFields contains two or more PivotField 
                pivotTable.AddFieldToArea(PivotFieldType.Column, pivotTable.DataField);
            }

            //add for layout
            int rowFieldsCount = pivotTable.RowFields.Count;
            for (int j = 0; j &lt; rowFieldsCount; j++)
            {
                PivotField f = pivotTable.RowFields[j];
                f.ShowCompact = true;
                f.ShowInOutlineForm = true;
                f.ShowSubtotalAtTop = true;
            }
            pivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium9;
            //end

            workbook.Save(Constants.PIVOT_CHECK_FILE_PATH + &quot;NET43877.xlsx&quot;);
        }
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


