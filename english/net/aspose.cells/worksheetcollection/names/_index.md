---
title: WorksheetCollection.Names
second_title: Aspose.Cells for .NET API Reference
description: WorksheetCollection property. Gets the collection of all the Name objects in the spreadsheet
type: docs
url: /net/aspose.cells/worksheetcollection/names/
---
## WorksheetCollection.Names property

Gets the collection of all the Name objects in the spreadsheet.

```csharp
public NameCollection Names { get; }
```

### Examples

```csharp
// Called: foreach (object no in wb.Worksheets.Names)
[Test]
        public void Property_Names()
        {
            for (int i = 1; i &lt; 3; i++)
            {
                Workbook wb = new Workbook(Constants.sourcePath + &quot;J42646_&quot; + i + &quot;.xls&quot;);
                Console.WriteLine(&quot;42646_&quot; + i + &quot;...&quot;);
                foreach (object no in wb.Worksheets.Names)
                {
                    string s = ((Name) no).RefersTo; //The inner exception should be ignored
                }
            }
        }
```

### See Also

* class [NameCollection](../../namecollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


