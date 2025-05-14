---
title: Workbook.HasRevisions
second_title: Aspose.Cells for .NET API Reference
description: Workbook property. Gets if the workbook has any tracked changes
type: docs
url: /net/aspose.cells/workbook/hasrevisions/
---
## Workbook.HasRevisions property

Gets if the workbook has any tracked changes

```csharp
public bool HasRevisions { get; }
```

### Examples

```csharp
// Called: Console.WriteLine(book.HasRevisions);
public void Workbook_Property_HasRevisions()
{
    Console.WriteLine("Workbook_Property_HasRevisions()");
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


