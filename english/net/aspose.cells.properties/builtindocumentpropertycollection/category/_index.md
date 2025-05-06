---
title: BuiltInDocumentPropertyCollection.Category
second_title: Aspose.Cells for .NET API Reference
description: BuiltInDocumentPropertyCollection property. Gets or sets the category of the document
type: docs
url: /net/aspose.cells.properties/builtindocumentpropertycollection/category/
---
## BuiltInDocumentPropertyCollection.Category property

Gets or sets the category of the document.

```csharp
public string Category { get; set; }
```

### Examples

```csharp
// Called: MyWb.BuiltInDocumentProperties.Category = &amp;quot;Category&amp;quot;;
[Test]
        // http://www.aspose.com/community/forums/thread/289627.aspx
        // Custom Labels in Bubble Chart Serie
        public void Property_Category()
        {
            Console.WriteLine(&quot;Property_Category()&quot;);
            string infn = path + @&quot;CELLSNET-25058\2bubble_chart_points.xlsx&quot;;
            string outfn = Constants.destPath + @&quot;CELLSNET-25058.xlsx&quot;;

            Workbook MyWb = new Workbook(infn);

            MyWb.BuiltInDocumentProperties.Title = &quot;Title&quot;;
            MyWb.BuiltInDocumentProperties.Category = &quot;Category&quot;;
            MyWb.BuiltInDocumentProperties.Comments = &quot;Comments&quot;;
            MyWb.BuiltInDocumentProperties.NameOfApplication = &quot;NameOfApplication&quot;;
            MyWb.BuiltInDocumentProperties.Company = &quot;Company&quot;;

            MyWb.Save(outfn);
        }
```

### See Also

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


