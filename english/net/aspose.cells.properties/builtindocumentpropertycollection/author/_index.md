---
title: BuiltInDocumentPropertyCollection.Author
second_title: Aspose.Cells for .NET API Reference
description: BuiltInDocumentPropertyCollection property. Gets or sets the name of the documents author
type: docs
url: /net/aspose.cells.properties/builtindocumentpropertycollection/author/
---
## BuiltInDocumentPropertyCollection.Author property

Gets or sets the name of the document's author.

```csharp
public string Author { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(&amp;quot;Aspose.Cells&amp;quot;, wb.BuiltInDocumentProperties.Author);
private void Property_Author(MemoryStream ms, int sheetCount)
        {
            ms.Seek(0, SeekOrigin.Begin);
            Workbook wb = new Workbook(ms, new LoadOptions()
            {
                LoadFilter = new LoadFilter(LoadDataFilterOptions.DocumentProperties)
            });
            Assert.AreEqual(&quot;Aspose.Cells&quot;, wb.BuiltInDocumentProperties.Author);
            Assert.AreEqual(&quot;MyVal&quot;, wb.CustomDocumentProperties[&quot;MyCustomProp&quot;].Value);
            //Assert.AreEqual(1, wb.Worksheets.Count, &quot;SheetCount&quot;);
            //Assert.AreEqual(-1, wb.Worksheets[0].Cells.MaxRow, &quot;MaxRow&quot;);
            //Assert.AreEqual(&quot;Sheet1&quot;, wb.Worksheets[0].Name, &quot;SheetName&quot;);
            ms.Seek(0, SeekOrigin.Begin);
            wb = new Workbook(ms, new LoadOptions()
            {
                LoadFilter = new LoadFilter(LoadDataFilterOptions.DocumentProperties | LoadDataFilterOptions.Structure)
            });
            Assert.AreEqual(&quot;Aspose.Cells&quot;, wb.BuiltInDocumentProperties.Author);
            Assert.AreEqual(&quot;MyVal&quot;, wb.CustomDocumentProperties[&quot;MyCustomProp&quot;].Value);
            Assert.AreEqual(sheetCount, wb.Worksheets.Count, &quot;SheetCount&quot;);
            Assert.AreEqual(-1, wb.Worksheets[0].Cells.MaxRow, &quot;MaxRow&quot;);
            Assert.AreEqual(&quot;st0&quot;, wb.Worksheets[0].Name, &quot;SheetName&quot;);
            Assert.AreEqual(&quot;st1&quot;, wb.Worksheets[1].Name, &quot;SheetName&quot;);
            ms.Seek(0, SeekOrigin.Begin);
            wb = new Workbook(ms, new LoadOptions()
            {
                LoadFilter = new LoadFilter(LoadDataFilterOptions.DocumentProperties
                    | LoadDataFilterOptions.CellData | LoadDataFilterOptions.DefinedNames)
            });
            Assert.AreEqual(&quot;Aspose.Cells&quot;, wb.BuiltInDocumentProperties.Author);
            Assert.AreEqual(&quot;MyVal&quot;, wb.CustomDocumentProperties[&quot;MyCustomProp&quot;].Value);
            Assert.AreEqual(sheetCount, wb.Worksheets.Count, &quot;SheetCount&quot;);
            Assert.AreEqual(0, wb.Worksheets[0].Cells.MaxRow, &quot;MaxRow&quot;);
            Assert.AreEqual(&quot;abc&quot;, wb.Worksheets[0].Cells[0, 0].Value, &quot;A1.Value&quot;);
            Assert.AreEqual(&quot;st0&quot;, wb.Worksheets[0].Name, &quot;SheetName&quot;);
            Assert.AreEqual(&quot;st1&quot;, wb.Worksheets[1].Name, &quot;SheetName&quot;);
        }
```

### See Also

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


