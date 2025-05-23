---
title: TxtLoadOptions.HasFormula
second_title: Aspose.Cells for .NET API Reference
description: TxtLoadOptions property. Indicates whether the text is formula if it starts with 
type: docs
url: /net/aspose.cells/txtloadoptions/hasformula/
---
## TxtLoadOptions.HasFormula property

Indicates whether the text is formula if it starts with "=".

```csharp
public bool HasFormula { get; set; }
```

### Examples

```csharp
// Called: options.HasFormula = true;
public void TxtLoadOptions_Property_HasFormula()
{
    TxtLoadOptions options = new TxtLoadOptions();
    options.HasFormula = true;
    options.SeparatorString = ("|");
    Workbook workbook = new Workbook(Constants.sourcePath  + "example.csv", options);
    Assert.AreEqual(workbook.Worksheets[0].Cells["K2"].Formula, "=\"000000000010775733\"");
    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


