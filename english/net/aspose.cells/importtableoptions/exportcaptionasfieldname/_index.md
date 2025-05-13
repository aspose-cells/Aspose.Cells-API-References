---
title: ImportTableOptions.ExportCaptionAsFieldName
second_title: Aspose.Cells for .NET API Reference
description: ImportTableOptions property. Indicates whether exporting caption as field name
type: docs
url: /net/aspose.cells/importtableoptions/exportcaptionasfieldname/
---
## ImportTableOptions.ExportCaptionAsFieldName property

Indicates whether exporting caption as field name

```csharp
public bool ExportCaptionAsFieldName { get; set; }
```

### Remarks

Only works for DataTable.

### Examples

```csharp
// Called: options.ExportCaptionAsFieldName = true;
public void ImportTableOptions_Property_ExportCaptionAsFieldName()
{
    List<Transaction>  transactions = new List<Transaction>();
    Transaction t = new Transaction();
    t.orderId = "w101";
    t.paymentType = "card";
    t.orderType = "bur";

    transactions.Add(t);
    transactions.Add(t);
    transactions.Add(t);
    transactions.Add(t);

    Workbook workbook = new Workbook();
    ImportTableOptions options = new ImportTableOptions();
    options.ExportCaptionAsFieldName = true;
    workbook.Worksheets[0].Cells.ImportCustomObjects(transactions, 0, 0, options);
    workbook.Save(Constants.destPath +@"example.xlsx");
    ExportTableOptions expOptions = new ExportTableOptions();
    List<Transaction> ret = workbook.Worksheets[0].Cells.ExportList<Transaction>(0, 0, 5, 10, expOptions);
    Assert.AreEqual(4, ret.Count);
    Assert.AreEqual("card", ret[0].paymentType);

}
```

### See Also

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


