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
// Called: externalLink.AddExternalName("Test", "=Sheet1!$B$2");
[Test, Category("Bug")]
        public void Method_String_()
        {
            Workbook workbook = new Workbook();
            string fileName = Constants.sourcePath + "ExternalName.xls";
            fileName = Path.GetFullPath(fileName);
            Workbook externalWorkbook = new Workbook(fileName);
            string[] sheetNames = new string[externalWorkbook.Worksheets.Count];
            for (int i = 0; i < externalWorkbook.Worksheets.Count; i++)
            {
                sheetNames[i] = externalWorkbook.Worksheets[i].Name;
            }
            int index = workbook.Worksheets.ExternalLinks.Add(fileName, sheetNames);
            ExternalLink externalLink = workbook.Worksheets.ExternalLinks[index];
            externalLink.AddExternalName("Test", "=Sheet1!$B$2");
            workbook.Worksheets[0].Cells["A1"].Formula = "=[" + fileName + "]!Test";
            workbook.UpdateLinkedDataSource(null);
            workbook.CalculateFormula();
            Assert.AreEqual(workbook.Worksheets[0].Cells["A1"].DoubleValue, 67);
            externalWorkbook.Worksheets["Sheet1"].Cells["B2"].PutValue("Hello");
            workbook.UpdateLinkedDataSource(new Workbook[] { externalWorkbook });
            workbook.CalculateFormula();
            Assert.AreEqual(workbook.Worksheets[0].Cells["A1"].StringValue, "Hello");
        }
```

### See Also

* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


