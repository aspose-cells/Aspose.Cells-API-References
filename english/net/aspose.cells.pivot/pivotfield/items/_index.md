---
title: PivotField.Items
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Get all labels of pivot items in this field
type: docs
url: /net/aspose.cells.pivot/pivotfield/items/
---
## PivotField.Items property

Get all labels of pivot items in this field.

```csharp
public string[] Items { get; }
```

### Examples

```csharp
// Called: string[] items = pivotField.Items;
private void PivotField_Property_Items(Worksheet worksheet, PivotTable pivotTable, PivotField pivotField, String field)
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


