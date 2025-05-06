---
title: WorkbookDesigner.ClearDataSource
second_title: Aspose.Cells for .NET API Reference
description: WorkbookDesigner method. Clears all data sources
type: docs
url: /net/aspose.cells/workbookdesigner/cleardatasource/
---
## WorkbookDesigner.ClearDataSource method

Clears all data sources.

```csharp
public void ClearDataSource()
```

### Examples

```csharp
// Called: myWorkbook.ClearDataSource();
[Test]
        public void Method_ClearDataSource()
        {
            WorkbookDesigner myWorkbook = new WorkbookDesigner();
            //myWorkbook.Open(xlFileName);
            Worksheet curentWorksheet = myWorkbook.Workbook.Worksheets[&quot;Sheet1&quot;];

            // Create temporary data
            IList&lt;Person&gt; myList = new List&lt;Person&gt;();
            myList.Add(new Person(&quot;X&quot;, 26));
            myList.Add(new Person(&quot;X&quot;, 32));
            myList.Add(new Person(&quot;Y&quot;, 19));


            // Set the headers and smart markers to the XL file
            curentWorksheet.Cells[&quot;A1&quot;].PutValue(&quot;Name&quot;);
            curentWorksheet.Cells[&quot;B1&quot;].PutValue(&quot;Age&quot;);
            curentWorksheet.Cells[&quot;A2&quot;].PutValue(&quot;&amp;=Person.Name(group:merge,skip:1)&quot;);
            curentWorksheet.Cells[&quot;B2&quot;].PutValue(&quot;&amp;=Person.Age&quot;);

            // Set the data to the XL sheet
            myWorkbook.SetDataSource(&quot;Person&quot;, myList);

            myWorkbook.Process();
            myWorkbook.ClearDataSource();
            myWorkbook.SetDataSource(&quot;Person&quot;, myList);
            myWorkbook.Workbook.Save(Constants.destPath + &quot;GroupCustomObjects.xls&quot;);
        }
```

### See Also

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


