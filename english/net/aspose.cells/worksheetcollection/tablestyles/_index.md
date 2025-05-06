---
title: WorksheetCollection.TableStyles
second_title: Aspose.Cells for .NET API Reference
description: WorksheetCollection property. Gets TableStyles object
type: docs
url: /net/aspose.cells/worksheetcollection/tablestyles/
---
## WorksheetCollection.TableStyles property

Gets `TableStyles` object.

```csharp
public TableStyleCollection TableStyles { get; }
```

### Examples

```csharp
// Called: Console.WriteLine(&amp;quot;tableStyles count: &amp;quot; + workbook.Worksheets.TableStyles.Count);
[Test]
        public void Property_TableStyles()
        {
            Console.WriteLine(&quot;Property_TableStyles()&quot;);
            string infn = path + &quot;Test_ImpExpCustomTableStyle.xlsx&quot;;
            string outfn = Constants.destPath + &quot;Test_ImpExpCustomTableStyle_out.xlsx&quot;;

            Workbook workbook = new Workbook(infn);
            Console.WriteLine(&quot;tableStyles count: &quot; + workbook.Worksheets.TableStyles.Count);
            workbook.Save(outfn);
        }
```

### See Also

* class [TableStyleCollection](../../../aspose.cells.tables/tablestylecollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


