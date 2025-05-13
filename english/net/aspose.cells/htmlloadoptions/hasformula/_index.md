---
title: HtmlLoadOptions.HasFormula
second_title: Aspose.Cells for .NET API Reference
description: HtmlLoadOptions property. Indicates whether the text is formula if it starts with 
type: docs
url: /net/aspose.cells/htmlloadoptions/hasformula/
---
## HtmlLoadOptions.HasFormula property

Indicates whether the text is formula if it starts with "=".

```csharp
public bool HasFormula { get; set; }
```

### Examples

```csharp
// Called: loadOptions.HasFormula = false;
public void HtmlLoadOptions_Property_HasFormula()
{
    HtmlLoadOptions loadOptions = new HtmlLoadOptions(LoadFormat.Html);
    loadOptions.ConvertNumericData = true;
    loadOptions.ConvertDateTimeData = false;
    loadOptions.HasFormula = false;
    loadOptions.IgnoreNotPrinted = true;
    loadOptions.SupportDivTag = true;

    loadOptions.AutoFitColsAndRows = true;

    //loadOptions.Encoding = System.Text.Encoding.GetEncoding("ISO-8859-1");


    // Create a Workbook object and opening the file from its path
    Workbook wb = new Workbook(Constants.HtmlPath + "example.html", loadOptions);

    Cells cells = wb.Worksheets[0].Cells;
    Assert.AreEqual("Daytime ", cells["A1"].StringValue);
    Assert.AreEqual("After-Hours", cells["B1"].StringValue);
    Assert.AreEqual("Backup", cells["C1"].StringValue);

    Assert.AreEqual("Employee Away Information", cells["A11"].StringValue);

    // Save the MHT file
    wb.Save(_destFilesPath + "example.xlsx");
}
```

### See Also

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


