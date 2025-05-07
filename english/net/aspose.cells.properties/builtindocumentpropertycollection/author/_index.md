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
// Called: wb.BuiltInDocumentProperties.Author = AuthorValue;
[Test]
        public void Property_Author()
        {
            Workbook wb = new Workbook(FileFormatType.Excel97To2003);

            string KeyAverageAge = "Average Age";
            double AverageAgeValue = 31.5;

            string KeyDistance = "Distance";
            float DistanceValue = 2194.5f;

            string AuthorValue = "John Smith";
            wb.BuiltInDocumentProperties.Author = AuthorValue;
            wb.CustomDocumentProperties.Add(KeyAverageAge, AverageAgeValue);
            wb.CustomDocumentProperties.Add(KeyDistance, DistanceValue);
            wb = Util.ReSave(wb, new XlsSaveOptions(), new LoadOptions(LoadFormat.Excel97To2003));
            Assert.AreEqual(AuthorValue, wb.BuiltInDocumentProperties.Author, "BuiltIn-Author");
            Assert.AreEqual(AverageAgeValue, wb.CustomDocumentProperties[KeyAverageAge].Value, "Custom-" + KeyAverageAge);
            Assert.AreEqual(DistanceValue, wb.CustomDocumentProperties[KeyDistance].Value, "Custom-" + KeyDistance);
        }
```

### See Also

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


