---
title: TxtSaveOptions.Separator
second_title: Aspose.Cells for .NET API Reference
description: TxtSaveOptions property. Gets and sets char Delimiter of text file
type: docs
url: /net/aspose.cells/txtsaveoptions/separator/
---
## TxtSaveOptions.Separator property

Gets and sets char Delimiter of text file.

```csharp
public char Separator { get; set; }
```

### Examples

```csharp
// Called: saveOptions.Separator = &amp;apos;,&amp;apos;;
[Test]
        public void Property_Separator()
        {
            string FileName = Constants.bugFilePath + &quot;ea.xls&quot;;
            Workbook workbook = new Workbook(FileName);
            TxtSaveOptions saveOptions = new TxtSaveOptions();
            saveOptions.Separator = &apos;,&apos;;
            workbook.Save(Constants.destPath + &quot;testSave.CSV&quot;, saveOptions);

            TxtLoadOptions loadOptions = new TxtLoadOptions();
            loadOptions.SeparatorString = &quot;,&quot;;
            workbook = new Workbook(Constants.destPath + &quot;testSave.CSV&quot;, loadOptions);
        }
```

### See Also

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


