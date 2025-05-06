---
title: TxtLoadOptions.Separator
second_title: Aspose.Cells for .NET API Reference
description: TxtLoadOptions property. Gets and sets character separator of text file
type: docs
url: /net/aspose.cells/txtloadoptions/separator/
---
## TxtLoadOptions.Separator property

Gets and sets character separator of text file.

```csharp
public char Separator { get; set; }
```

### Examples

```csharp
// Called: txtLoadOption.Separator = &amp;apos; &amp;apos;;
[Test, Category(&quot;Bug&quot;)]
        public void Property_Separator()
        {
            Workbook workbook = new Workbook();
            //workbook.Open(Constants.sourcePath +&quot;TOF129.TXT&quot;, &apos; &apos;);
            TxtLoadOptions txtLoadOption = new TxtLoadOptions();
            txtLoadOption.Separator = &apos; &apos;;
            workbook = new Workbook(Constants.sourcePath + &quot;TOF129.TXT&quot;, txtLoadOption);
            Assert.AreEqual(workbook.Worksheets[0].Cells[&quot;B13&quot;].StringValue, &quot;LIMITS&quot;);
        }
```

### See Also

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


