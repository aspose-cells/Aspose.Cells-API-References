---
title: PivotField.CurrentPageItem
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Represents the current page item showing for the page field valid only for page fields
type: docs
url: /net/aspose.cells.pivot/pivotfield/currentpageitem/
---
## PivotField.CurrentPageItem property

Represents the current page item showing for the page field (valid only for page fields).

```csharp
public short CurrentPageItem { get; set; }
```

### Examples

```csharp
// Called: selectedField.CurrentPageItem =(short) iIndexValue;
[Test]
        public void Property_CurrentPageItem()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;NET45254_&quot;;

            Workbook workbook = new Workbook(filePath + @&quot;Template.xlsm&quot;);
            Worksheet selectedSheet = workbook.Worksheets[&quot;Data&quot;];
            DataTable dt = new DataTable();
            dt.ReadXml(filePath + &quot;27f1f764-401c-4077-88d6-fa49698d5ddc.xml&quot;);
            selectedSheet.Cells.ImportData(dt, 1, 0, new ImportTableOptions() { IsFieldNameShown = false });
            selectedSheet = workbook.Worksheets[&quot;Exposure&quot;];
            int iIndex = selectedSheet.PivotTables.Add(&quot;=&apos;Data&apos;!A1:CK37&quot;, &quot;A5&quot;, &quot;IRIS010_pivot&quot;);
            PivotTable selectedPivotTable = selectedSheet.PivotTables[iIndex];
            iIndex = selectedPivotTable.AddFieldToArea(PivotFieldType.Page, &quot;Is Fixing Cur&quot;);
            PivotField selectedField = selectedPivotTable.PageFields[iIndex];
            //string[] filtersValues = { &quot;Y&quot; }; /*  for sample is Y but depending on user settings you can have multiple values here, and the problem comes when only one */
            ArrayList filtersValues = new ArrayList();
            filtersValues.Add(&quot;Y&quot;);
            selectedField.IsMultipleItemSelectionAllowed = filtersValues.Count &gt; 1;
            string[] pItems = selectedField.Items;
            for (short iIndexValue = 0; iIndexValue &lt; pItems.Length; iIndexValue++)
            {
                bool isHidden = !filtersValues.Contains(pItems[iIndexValue]);
                if(!isHidden)
                {
                    if (!selectedField.IsMultipleItemSelectionAllowed)
                    {
                        selectedField.CurrentPageItem =(short) iIndexValue;
                    }
                  
                }
                selectedField.HideItem(iIndexValue, isHidden);

            }
            iIndex = selectedPivotTable.AddFieldToArea(PivotFieldType.Column, &quot;Cur&quot;);

            iIndex = selectedPivotTable.AddFieldToArea(PivotFieldType.Row, &quot;Hedge&quot;);

            iIndex = selectedPivotTable.AddFieldToArea(PivotFieldType.Row, &quot;Hedge Name&quot;);

            iIndex = selectedPivotTable.AddFieldToArea(PivotFieldType.Row, &quot;Fixing Date&quot;);

            iIndex = selectedPivotTable.AddFieldToArea(PivotFieldType.Data, &quot;Amount&quot;);

            selectedPivotTable.RefreshData();
            selectedPivotTable.CalculateRange();
            selectedPivotTable.CalculateData();

            Assert.AreEqual(selectedSheet.Cells[&quot;B3&quot;].StringValue, &quot;Y&quot;);
            workbook.Save(CreateFolder(filePath) + @&quot;out.xlsx&quot;);
        }
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


