---
title: Workbook.AcceptAllRevisions
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Accepts all tracked changes in the workbook
type: docs
url: /net/aspose.cells/workbook/acceptallrevisions/
---
## Workbook.AcceptAllRevisions method

Accepts all tracked changes in the workbook.

```csharp
public void AcceptAllRevisions()
```

### Examples

```csharp
// Called: book.AcceptAllRevisions();
[Test]
        public void Method_AcceptAllRevisions()
        {
            Console.WriteLine("Method_AcceptAllRevisions()");
            string infn = path + "Test_Revision.xlsx";
            string outfn1 = Constants.destPath + "Test_Revision_out.xlsx";
            string outfn2 = Constants.destPath + "Test_Revision_out_noRevison.xlsx";

            Workbook book = new Workbook(infn);
            book.Save(outfn1);

            book = new Workbook(infn);
            Console.WriteLine(book.HasRevisions);
            book.AcceptAllRevisions();
            Console.WriteLine(book.HasRevisions);
            book.Save(outfn2);
        }
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


