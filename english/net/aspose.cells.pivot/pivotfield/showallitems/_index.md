---
title: PivotField.ShowAllItems
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Indicates whether all items displays in the PivotTable report even if they dont contain summary data. show items with no data The default value is false
type: docs
url: /net/aspose.cells.pivot/pivotfield/showallitems/
---
## PivotField.ShowAllItems property

Indicates whether all items displays in the PivotTable report, even if they don't contain summary data. show items with no data The default value is false.

```csharp
public bool ShowAllItems { get; set; }
```

### Examples

```csharp
// Called: pt_demo.PageFields[1].ShowAllItems = true;
[Test]
        public void Property_ShowAllItems()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;JAVA42750_&quot;;

            Workbook wb_demo = new Workbook(filePath + &quot;Efficiency Test Data.xlsx&quot;);
            PivotTable pt_demo = wb_demo.Worksheets[1].PivotTables[0];
            Console.WriteLine(pt_demo.Name);
            pt_demo.RefreshData();

            pt_demo.PageFields[1].ShowAllItems = true;
            //Get the second Pivot page field 
            PivotField src_t_field = pt_demo.PageFields[1];
            src_t_field.IsMultipleItemSelectionAllowed = true;

            Console.WriteLine(src_t_field.Name);//Audited_By - Ok 
            Console.WriteLine(&quot;Total Items: &quot; + src_t_field.Items.Length);//0 - Not Ok 
            Console.WriteLine(&quot;Total Items: &quot; + src_t_field.PivotItems.Count);//0 - Not Ok 

            //pt_demo.refreshData(); 

            //This code segment is for no use 
            PivotItemCollection collection_src_t = src_t_field.PivotItems;
            for (int i = 0; i &lt; collection_src_t.Count; i++)
            {
                PivotItem item = collection_src_t[i];
                Console.WriteLine(item.Name);
            }
        }
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


