---
title: OleObject.IsAutoSize
second_title: Aspose.Cells for .NET API Reference
description: OleObject property. True indicates that the size of the ole object will be auto changed as the size of snapshot of the embedded content when the ole object is activated
type: docs
url: /net/aspose.cells.drawing/oleobject/isautosize/
---
## OleObject.IsAutoSize property

True indicates that the size of the ole object will be auto changed as the size of snapshot of the embedded content when the ole object is activated.

```csharp
public bool IsAutoSize { get; set; }
```

### Examples

```csharp
// Called: book.Worksheets[0].OleObjects[0].IsAutoSize = true;
[Test]
        public void Property_IsAutoSize()
        {
            Console.WriteLine("Property_IsAutoSize()");
            string infn = path + "Test_OleObjectIsAutoSize.xls";
            string outfn = Constants.destPath + "Test_OleObjectIsAutoSize_out.xlsx";
            string outfn1 = Constants.destPath + "Test_OleObjectIsAutoSize_true.xlsx";
            string outfn2 = Constants.destPath + "Test_OleObjectIsAutoSize_false.xlsx";

            Workbook book = new Workbook(infn);
            book.Save(outfn);
            book.Worksheets[0].OleObjects[0].IsAutoSize = true;
            book.Save(outfn1);
            book.Worksheets[0].OleObjects[0].IsAutoSize = false;
            book.Save(outfn2);

            Workbook book1 = new Workbook(outfn1);
            if (!book1.Worksheets[0].OleObjects[0].IsAutoSize)
                throw new Exception("Property_IsAutoSize() failed!");
            Workbook book2 = new Workbook(outfn2);
            if (book2.Worksheets[0].OleObjects[0].IsAutoSize)
                throw new Exception("Property_IsAutoSize() failed!");
        }
```

### See Also

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


