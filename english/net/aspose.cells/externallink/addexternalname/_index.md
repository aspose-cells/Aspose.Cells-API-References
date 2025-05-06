---
title: ExternalLink.AddExternalName
second_title: Aspose.Cells for .NET API Reference
description: ExternalLink method. Adds an external name
type: docs
url: /net/aspose.cells/externallink/addexternalname/
---
## ExternalLink.AddExternalName method

Adds an external name.

```csharp
public void AddExternalName(string text, string referTo)
```

| Parameter | Type | Description |
| --- | --- | --- |
| text | String | The text of the external name. If the external name belongs to a worksheet, the text should be as Sheet1!Text. |
| referTo | String | The referTo of the external name. It must be a cell or the range. |

### Examples

```csharp
// Called: externalLink.AddExternalName(&amp;quot;Test&amp;quot;, &amp;quot;=Sheet1!$B$2&amp;quot;);
[Test, Category(&quot;Bug&quot;)]
        public void Method_String_()
        {
            Workbook workbook = new Workbook();
            string fileName = Constants.sourcePath + &quot;ExternalName.xls&quot;;
            fileName = Path.GetFullPath(fileName);
            Workbook externalWorkbook = new Workbook(fileName);
            string[] sheetNames = new string[externalWorkbook.Worksheets.Count];
            for (int i = 0; i &lt; externalWorkbook.Worksheets.Count; i++)
            {
                sheetNames[i] = externalWorkbook.Worksheets[i].Name;
            }
            int index = workbook.Worksheets.ExternalLinks.Add(fileName, sheetNames);
            ExternalLink externalLink = workbook.Worksheets.ExternalLinks[index];
            externalLink.AddExternalName(&quot;Test&quot;, &quot;=Sheet1!$B$2&quot;);
            workbook.Worksheets[0].Cells[&quot;A1&quot;].Formula = &quot;=[&quot; + fileName + &quot;]!Test&quot;;
            workbook.UpdateLinkedDataSource(null);
            workbook.CalculateFormula();
            Assert.AreEqual(workbook.Worksheets[0].Cells[&quot;A1&quot;].DoubleValue, 67);
            externalWorkbook.Worksheets[&quot;Sheet1&quot;].Cells[&quot;B2&quot;].PutValue(&quot;Hello&quot;);
            workbook.UpdateLinkedDataSource(new Workbook[] { externalWorkbook });
            workbook.CalculateFormula();
            Assert.AreEqual(workbook.Worksheets[0].Cells[&quot;A1&quot;].StringValue, &quot;Hello&quot;);
        }
```

### See Also

* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


