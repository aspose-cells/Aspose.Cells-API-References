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
// Called: pivotField.CurrentPageItem = (short)list.IndexOf("(blank)");
private void Property_CurrentPageItem(Worksheet worksheet, PivotTable pivotTable, PivotField pivotField, String field)
        {
            string[] items = pivotField.Items;
            ArrayList list = new ArrayList(items);
            //Console.WriteLine("Fields are: " + Arrays.asList(pivotField.getItems()));
            if (list.Contains(field))
            {
                pivotField.CurrentPageItem = (short)list.IndexOf(field);
                //System.out.println("Current page item set for" + field + "is:" + pivotField.getCurrentPageItem() + pivotField.getItems());
            }
            else
            {
                pivotField.CurrentPageItem = (short)list.IndexOf("(blank)");
                //System.out.println("Current page item set for (blank) is:" + pivotField.getCurrentPageItem() + pivotField.getItems());
            }
            pivotTable.CalculateData();
            //pivotTable.RefreshDataOnOpeningFile = true;
        }
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


