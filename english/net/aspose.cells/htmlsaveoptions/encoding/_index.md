---
title: HtmlSaveOptions.Encoding
second_title: Aspose.Cells for .NET API Reference
description: HtmlSaveOptions property. If not setuse Encoding.UTF8 as default enconding type
type: docs
url: /net/aspose.cells/htmlsaveoptions/encoding/
---
## HtmlSaveOptions.Encoding property

If not set,use Encoding.UTF8 as default enconding type.

```csharp
public Encoding Encoding { get; set; }
```

### Examples

```csharp
// Called: sopts.Encoding = Encoding.UTF8;
public void HtmlSaveOptions_Property_Encoding()
{
    Workbook wb = new Workbook();
    wb.Worksheets[0].Cells[0, 0].PutValue("this is first sheet");
    wb.Worksheets.Add("Sheet2").Cells[0, 0].PutValue("this is second sheet");
    HtmlSaveOptions sopts = new HtmlSaveOptions();
    MemoryStream ms1 = new MemoryStream();
    MemoryStream ms2 = new MemoryStream();
    sopts.Encoding = Encoding.UTF8;
    SaveSheetStreamProvider provider = new SaveSheetStreamProvider(ms1, ms2);
    sopts.StreamProvider = provider;
    wb.Save(new MemoryStream(), sopts);
    Assert.AreEqual(provider.InitCount, provider.CloseCount, "Init count should be same with closed count");
    string result = Encoding.UTF8.GetString(ms1.GetBuffer(), 0, (int)ms1.Length);
    if (result.IndexOf("this is first sheet") < 0)
    {
        Assert.Fail("There is no expected cell value in ms1 whose length is " + ms1.Length);
    }
    result = Encoding.UTF8.GetString(ms2.GetBuffer(), 0, (int)ms2.Length);
    if (result.IndexOf("this is second sheet") < 0)
    {
        Assert.Fail("There is no expected cell value in ms1 whose length is " + ms1.Length);
    }
}
```

### See Also

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


