---
title: PivotField.PivotItems
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Gets the pivot items of the pivot field
type: docs
url: /net/aspose.cells.pivot/pivotfield/pivotitems/
---
## PivotField.PivotItems property

Gets the pivot items of the pivot field

```csharp
public PivotItemCollection PivotItems { get; }
```

### Examples

```csharp
// Called: PivotItemCollection collection_src_t = src_t_field.PivotItems;
[Test]
        public void Property_PivotItems()
        {
            string filePath = Constants.PivotTableSourcePath + @"JAVA42750_";

            Workbook wb_demo = new Workbook(filePath + "Efficiency Test Data.xlsx");
            PivotTable pt_demo = wb_demo.Worksheets[1].PivotTables[0];
            Console.WriteLine(pt_demo.Name);
            pt_demo.RefreshData();

            pt_demo.PageFields[1].ShowAllItems = true;
            //Get the second Pivot page field 
            PivotField src_t_field = pt_demo.PageFields[1];
            src_t_field.IsMultipleItemSelectionAllowed = true;

            Console.WriteLine(src_t_field.Name);//Audited_By - Ok 
            Console.WriteLine("Total Items: " + src_t_field.Items.Length);//0 - Not Ok 
            Console.WriteLine("Total Items: " + src_t_field.PivotItems.Count);//0 - Not Ok 

            //pt_demo.refreshData(); 

            //This code segment is for no use 
            PivotItemCollection collection_src_t = src_t_field.PivotItems;
            for (int i = 0; i < collection_src_t.Count; i++)
            {
                PivotItem item = collection_src_t[i];
                Console.WriteLine(item.Name);
            }
        }
```

### See Also

* class [PivotItemCollection](../../pivotitemcollection/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


