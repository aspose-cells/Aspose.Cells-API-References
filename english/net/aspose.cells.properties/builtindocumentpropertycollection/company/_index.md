---
title: BuiltInDocumentPropertyCollection.Company
second_title: Aspose.Cells for .NET API Reference
description: BuiltInDocumentPropertyCollection property. Gets or sets the company property
type: docs
url: /net/aspose.cells.properties/builtindocumentpropertycollection/company/
---
## BuiltInDocumentPropertyCollection.Company property

Gets or sets the company property.

```csharp
public string Company { get; set; }
```

### Examples

```csharp
// Called: MyWb.BuiltInDocumentProperties.Company = "Company";
// http://www.aspose.com/community/forums/thread/289627.aspx
// Custom Labels in Bubble Chart Serie
public void BuiltInDocumentPropertyCollection_Property_Company()
{
    Console.WriteLine("BuiltInDocumentPropertyCollection_Property_Company()");
    string infn = path + @"example.xlsx";
    string outfn = Constants.destPath + @"example.xlsx";

    Workbook MyWb = new Workbook(infn);

    MyWb.BuiltInDocumentProperties.Title = "Title";
    MyWb.BuiltInDocumentProperties.Category = "Category";
    MyWb.BuiltInDocumentProperties.Comments = "Comments";
    MyWb.BuiltInDocumentProperties.NameOfApplication = "NameOfApplication";
    MyWb.BuiltInDocumentProperties.Company = "Company";

    MyWb.Save(outfn);
}
```

### See Also

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


