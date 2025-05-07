---
title: AbstractTextLoadOptions.Encoding
second_title: Aspose.Cells for .NET API Reference
description: AbstractTextLoadOptions property. Gets and sets the default encoding. Only applies for csv file
type: docs
url: /net/aspose.cells/abstracttextloadoptions/encoding/
---
## AbstractTextLoadOptions.Encoding property

Gets and sets the default encoding. Only applies for csv file.

```csharp
public Encoding Encoding { get; set; }
```

### Examples

```csharp
// Called: options.Encoding = Encoding.UTF8;
[Test]
        public void Property_Encoding()
        {
            string source = Constants.PAGESETUP_FORMATTING_PATH + "pagesetup2003_single.htm";
            string dest = _destFilesPath + @"pagesetup2003_single_outhtm.htm";
            HtmlLoadOptions options = new HtmlLoadOptions(LoadFormat.Html);
            options.Encoding = Encoding.UTF8;
            Workbook wb = new Workbook(source, options);
            wb.Save(dest, SaveFormat.Html);

            CompareOption option = InitCompareOption();
            CompareAction.Compare(source, dest, option);
        }
```

### See Also

* class [AbstractTextLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


