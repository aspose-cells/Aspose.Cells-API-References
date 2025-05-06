---
title: LoadOptions.Password
second_title: Aspose.Cells for .NET API Reference
description: LoadOptions property. Gets and set the password of the workbook
type: docs
url: /net/aspose.cells/loadoptions/password/
---
## LoadOptions.Password property

Gets and set the password of the workbook.

```csharp
public string Password { get; set; }
```

### Examples

```csharp
// Called: loadOptions.Password = &amp;quot;1234&amp;quot;;
[Test]
        public void Property_Password()
        {
            Workbook workbook = new Workbook();

            //workbook.Open(Constants.sourcePath + &quot;TestEncrypt2007.xlsx&quot;, FileFormatType.Excel2007Xlsx, &quot;1234&quot;);
            LoadOptions loadOptions = new LoadOptions(LoadFormat.Xlsx);
            loadOptions.Password = &quot;1234&quot;;
            workbook = new Workbook(Constants.sourcePath + &quot;TestEncrypt2007.xlsx&quot;, loadOptions);

            workbook.Save(Constants.destPath + &quot;TestEncrypt2007.xlsx&quot;);
        }
```

### See Also

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


