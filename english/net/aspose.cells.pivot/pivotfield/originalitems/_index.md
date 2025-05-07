---
title: PivotField.OriginalItems
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Get the original base items
type: docs
url: /net/aspose.cells.pivot/pivotfield/originalitems/
---
## PivotField.OriginalItems property

Get the original base items;

```csharp
public string[] OriginalItems { get; }
```

### Examples

```csharp
// Called: string[] t = field.OriginalItems;
[Test]
        public void Property_OriginalItems()
        {
            Workbook wb = new Workbook(Constants.openPivottablePath + "AsposeItemsCache.xlsx");
            PivotFieldCollection fields = wb.Worksheets[0].PivotTables[0].BaseFields;
            for (int i = 0; i < fields.Count; i++)
            {
                PivotField field = fields[i];
                string[] t = field.OriginalItems;
                for (int j = 0; j < t.Length; j++)
                    Console.WriteLine(t[j]);
            }
            //wb.Save("D:\\tttt.xlsx");
        }
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


