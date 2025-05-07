---
title: CustomDocumentPropertyCollection.UpdateLinkedPropertyValue
second_title: Aspose.Cells for .NET API Reference
description: CustomDocumentPropertyCollection method. Update custom document property value which links to content
type: docs
url: /net/aspose.cells.properties/customdocumentpropertycollection/updatelinkedpropertyvalue/
---
## CustomDocumentPropertyCollection.UpdateLinkedPropertyValue method

Update custom document property value which links to content.

```csharp
public void UpdateLinkedPropertyValue()
```

### Examples

```csharp
// Called: workbook.CustomDocumentProperties.UpdateLinkedPropertyValue();
[Test]
        // Various Custom Property issues when using xls and xlsx/xlsm documents
        // http://www.aspose.com/community/forums/thread/291663.aspx
        public void Method_UpdateLinkedPropertyValue()
        {
            Console.WriteLine("Method_UpdateLinkedPropertyValue()");
            string infn03 = path + @"CELLSNET-25332\CustPropTest_2003.xls";
            string outfn03 = Constants.destPath + @"CELLSNET-25332_2003_out.xls";
            string infn07 = path + @"CELLSNET-25332\CustPropTest_2007.xlsx";
            string outfn07 = Constants.destPath + @"CELLSNET-25332_2007_out.xlsx";
            string infn10 = path + @"CELLSNET-25332\CustPropTest_2010.xlsx";
            string outfn10 = Constants.destPath + @"CELLSNET-25332_2010_out.xlsx";

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

* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


