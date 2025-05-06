---
title: PivotItem.Name
second_title: Aspose.Cells for .NET API Reference
description: PivotItem property. Gets the name of the pivot item
type: docs
url: /net/aspose.cells.pivot/pivotitem/name/
---
## PivotItem.Name property

Gets the name of the pivot item.

```csharp
public string Name { get; set; }
```

### Examples

```csharp
// Called: if ((item.Name != null) &amp;amp;&amp;amp; item.Name.Equals(&amp;quot;CCC&amp;quot;))
[Test]
        public void Property_Name()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;JAVA41817_&quot;;

            Workbook wb_demo = new Workbook(filePath + &quot;Book2.xlsx&quot;);
            PivotTable pt_demo = wb_demo.Worksheets[0].PivotTables[0];
            pt_demo.ColumnFields[0].ShowAllItems = true;
            pt_demo.DataFields[0].ShowAllItems = true;

            PivotField src_t_field = pt_demo.PageFields[0];
            src_t_field.IsMultipleItemSelectionAllowed = true;
            //pt_demo.getColumnFields().get(0).setShowAllItems(true); 

            pt_demo.RefreshData();

            PivotItemCollection collection_src_t = src_t_field.PivotItems;

            for (int i = 0; i &lt; collection_src_t.Count; i++)
            {
                PivotItem item = collection_src_t[i];
                Console.WriteLine(item.Name);
                if ((item.Name != null) &amp;&amp; item.Name.Equals(&quot;CCC&quot;))
                {
                    Console.WriteLine(item.Name + &quot; src selected&quot;);
                    item.IsHidden = false;
                }
                else
                {
                    item.IsHidden = true;
                }
            }
            pt_demo.RefreshData();
            pt_demo.CalculateData();

            for (int i = 0; i &lt; pt_demo.BaseFields.Count; i++)
            {
                pt_demo.BaseFields[i].ShowAllItems = true;
                Console.WriteLine(pt_demo.BaseFields[i].Name);
            }
            /* 
            pt_demo.getColumnFields().get(0).setShowAllItems(true); 
            System.out.println(pt_demo.getColumnFields().get(0).getName()); 
            pt_demo.getDataFields().get(0).setShowAllItems(true); 
            System.out.println(pt_demo.getDataFields().get(0).getName()); 
            pt_demo.getRowFields().get(0).setShowAllItems(true); 
            System.out.println(pt_demo.getRowFields().get(0).getName()); 
            pt_demo.getDataFields().get(0).setShowAllItems(true); 
            System.out.println(pt_demo.getDataFields().get(0).getName()); 
            */

            pt_demo.RowFields[0].ShowAllItems = true;
            Console.WriteLine(pt_demo.RowFields[0].Name);

            pt_demo.RefreshData();
            pt_demo.CalculateData();

            Cell lastDCell = wb_demo.Worksheets[0].Cells.EndCellInColumn((short)0);

            for (int row = 1; row &lt;= lastDCell.Row; row++)
            {
                //System.out.println(row+&quot; &quot;+lastFCell.getRow()); 
                Cell cell0 = wb_demo.Worksheets[0].Cells[row, 0];
                Cell cell1 = wb_demo.Worksheets[0].Cells[row, 1];
                Cell cell2 = wb_demo.Worksheets[0].Cells[row, 2];
                Cell cell3 = wb_demo.Worksheets[0].Cells[row, 3];
                Cell cell4 = wb_demo.Worksheets[0].Cells[row, 4];

                Console.WriteLine(&quot;Demo &quot; + cell0.Value + &quot; &quot;
                        + cell1.Value + &quot; &quot;
                        + cell2.Value + &quot; &quot;
                        + cell3.Value + &quot; &quot;
                        + cell4.Value + &quot; &quot;
                        );

            }
            Assert.AreEqual(wb_demo.Worksheets[0].Cells[4, 0].StringValue, &quot;xxx&quot;);
            Assert.AreEqual(wb_demo.Worksheets[0].Cells[5, 0].StringValue, &quot;yyy&quot;);
            Assert.AreEqual(wb_demo.Worksheets[0].Cells[6, 0].StringValue, &quot;zzz&quot;);
            wb_demo.Save(Constants.PivotTableDestPath + @&quot;JAVA41817.xlsx&quot;);
        }
```

### See Also

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


