---
title: PivotTable.DataFieldHeaderName
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Gets and sets the name of the value area field header in the PivotTable
type: docs
url: /net/aspose.cells.pivot/pivottable/datafieldheadername/
---
## PivotTable.DataFieldHeaderName property

Gets and sets the name of the value area field header in the PivotTable.

```csharp
public string DataFieldHeaderName { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(&amp;quot;Data&amp;quot;, workbook.Worksheets[1].PivotTables[0].DataFieldHeaderName);
[Test]
        //http://www.aspose.com/community/forums/thread/307686.aspx
        public void Property_DataFieldHeaderName()
        {
            Console.WriteLine(&quot;Property_DataFieldHeaderName()&quot;);
            string infn = path + @&quot;CELLSNET-27993\PivotTest.xls&quot;;
            string outfn1 = destpath + @&quot;CELLSNET27993_out1.xls&quot;;
            string outfn2 = destpath + @&quot;CELLSNET27993_out2.xlsx&quot;;

            Workbook workbook = new Workbook(infn);
            Assert.AreEqual(&quot;PivotTable1&quot;, workbook.Worksheets[1].PivotTables[0].Name);
            Assert.AreEqual(&quot;Data&quot;, workbook.Worksheets[1].PivotTables[0].DataFieldHeaderName);
            workbook.Save(outfn1);
            workbook.Save(outfn2);

        }
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


