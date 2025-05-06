---
title: PivotField.IsIncludeNewItemsInFilter
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Indicates whether including new items to the field in manual filter. The default value is false
type: docs
url: /net/aspose.cells.pivot/pivotfield/isincludenewitemsinfilter/
---
## PivotField.IsIncludeNewItemsInFilter property

Indicates whether including new items to the field in manual filter. The default value is false.

```csharp
public bool IsIncludeNewItemsInFilter { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(field.IsIncludeNewItemsInFilter, true);
[Test]
        public void Property_IsIncludeNewItemsInFilter()
        {
            Workbook wb = new Workbook(Constants.openPivottablePath + &quot;AsposeIsIncludeNewItemsInFilter.xls&quot;);
            PivotTable table = wb.Worksheets[1].PivotTables[0];
            PivotField field = table.RowFields[0];

            Assert.AreEqual(field.IsIncludeNewItemsInFilter, true);

            //Console.WriteLine(field.IsIncludeNewItemsInFilter);
            //Console.WriteLine(field.IsRepeatItemLabels);
            //Console.WriteLine(field.ShowAllItems);
            //Console.WriteLine(field.IsInsertPageBreaksBetweenItems);

            //Console.WriteLine(table.Indent);
            //Console.WriteLine(table.IsMultipleFieldFilters);
            //Console.WriteLine(table.ShowDataTips);
            //Console.WriteLine(table.ShowMemberPropertyTips);
            //Console.WriteLine(table.ShowValuesRow);
            //Console.WriteLine(table.ShowEmptyRow);
            //Console.WriteLine(table.ShowEmptyCol);
            //Console.WriteLine(table.FieldListSortAscending);
            //Console.WriteLine(table.ShowDrill);
            //Console.WriteLine(table.MissingItemsLimit);
            //Console.WriteLine(table.EnableDataValueEditing);
            //Console.WriteLine(table.AltTextTitle);
            //Console.WriteLine(table.AltTextDescription);
        }
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


