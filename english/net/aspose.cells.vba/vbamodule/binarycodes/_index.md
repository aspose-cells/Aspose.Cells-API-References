---
title: VbaModule.BinaryCodes
second_title: Aspose.Cells for .NET API Reference
description: VbaModule property. Gets and sets the binary codes of module
type: docs
url: /net/aspose.cells.vba/vbamodule/binarycodes/
---
## VbaModule.BinaryCodes property

Gets and sets the binary codes of module.

```csharp
public byte[] BinaryCodes { get; }
```

### Examples

```csharp
// Called: byte[] codes = p.Modules[0].BinaryCodes;
[Test]
        public void Property_BinaryCodes()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;CELLSJAVA46274.xlsm&quot;);
            VbaProject p = wb.VbaProject;
            byte[] codes = p.Modules[0].BinaryCodes;
            string str = Encoding.GetEncoding(936).GetString(codes);
            Assert.IsTrue(str.IndexOf(&quot;测试&quot;) != -1);
        }
```

### See Also

* class [VbaModule](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


