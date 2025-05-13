---
title: DocumentProperty.IsLinkedToContent
second_title: Aspose.Cells for .NET API Reference
description: DocumentProperty property. Indicates whether this property is linked to content
type: docs
url: /net/aspose.cells.properties/documentproperty/islinkedtocontent/
---
## DocumentProperty.IsLinkedToContent property

Indicates whether this property is linked to content

```csharp
public bool IsLinkedToContent { get; }
```

### Examples

```csharp
// Called: Assert.IsTrue(docProp.IsLinkedToContent);
// Various Custom Property issues when using xls and xlsx/xlsm documents
// http://www.aspose.com/community/forums/thread/291663.aspx
public void DocumentProperty_Property_IsLinkedToContent()
{
    Console.WriteLine("DocumentProperty_Property_IsLinkedToContent()");
    string infn03 = path + @"example.xls";
    string outfn03 = Constants.destPath + @"example.xls";
    string infn07 = path + @"example.xlsx";
    string outfn07 = Constants.destPath + @"example.xlsx";
    string infn10 = path + @"example.xlsx";
    string outfn10 = Constants.destPath + @"example.xlsx";

    Workbook workbook = new Workbook(infn03);
    Cell currentCell = workbook.Worksheets[0].Cells[0, 0];
    currentCell.Value = "Test1_updated";

    currentCell = workbook.Worksheets[0].Cells[0, 1];
    currentCell.Value = "Test2_updated";

    workbook.CustomDocumentProperties.UpdateLinkedPropertyValue();

    DocumentProperty docProp = workbook.CustomDocumentProperties[0];
    Assert.IsTrue(docProp.IsLinkedToContent);
    Assert.AreEqual("CPY_NAME", docProp.Source);
    Assert.AreEqual("Test1_updated", docProp.Value);

    docProp = null;
    docProp = workbook.CustomDocumentProperties[2];
    Assert.IsTrue(docProp.IsLinkedToContent);
    Assert.AreEqual("CO_NAME", docProp.Source);
    Assert.AreEqual("Test2_updated", docProp.Value);

    workbook.Save(outfn03);

    workbook = null;
    currentCell = null;

    workbook = new Workbook(infn07);
    currentCell = workbook.Worksheets[0].Cells[0, 0];
    currentCell.Value = "Test1_updated";

    currentCell = workbook.Worksheets[0].Cells[0, 1];
    currentCell.Value = "Test2_updated";

    workbook.CustomDocumentProperties.UpdateLinkedPropertyValue();

    docProp = null;
    docProp = workbook.CustomDocumentProperties[0];
    Assert.IsTrue(docProp.IsLinkedToContent);
    Assert.AreEqual("CPY_NAME", docProp.Source);
    Assert.AreEqual("Test1_updated", docProp.Value);

    docProp = null;
    docProp = workbook.CustomDocumentProperties[2];
    Assert.IsTrue(docProp.IsLinkedToContent);
    Assert.AreEqual("CO_NAME", docProp.Source);
    Assert.AreEqual("Test2_updated", docProp.Value);

    workbook.Save(outfn07);

    workbook = null;
    currentCell = null;

    workbook = new Workbook(infn10);
    currentCell = workbook.Worksheets[0].Cells[0, 0];
    currentCell.Value = "Test1_updated";

    currentCell = workbook.Worksheets[0].Cells[0, 1];
    currentCell.Value = "Test2_updated";

    workbook.CustomDocumentProperties.UpdateLinkedPropertyValue();

    docProp = null;
    docProp = workbook.CustomDocumentProperties[0];
    Assert.IsTrue(docProp.IsLinkedToContent);
    Assert.AreEqual("CPY_NAME", docProp.Source);
    Assert.AreEqual("Test1_updated", docProp.Value);

    docProp = null;
    docProp = workbook.CustomDocumentProperties[2];
    Assert.IsTrue(docProp.IsLinkedToContent);
    Assert.AreEqual("CO_NAME", docProp.Source);
    Assert.AreEqual("Test2_updated", docProp.Value);

    workbook.Save(outfn10);
}
```

### See Also

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


