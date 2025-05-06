---
title: Hyperlink.Address
second_title: Aspose.Cells for .NET API Reference
description: Hyperlink property. Represents the address of a hyperlink
type: docs
url: /net/aspose.cells/hyperlink/address/
---
## Hyperlink.Address property

Represents the address of a hyperlink.

```csharp
public string Address { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(workbook.Worksheets[0].Hyperlinks[0].Address, &amp;quot;http://dev.dms.firstam.com/title/documents/work instructions/title/california/ca-res full search/full search write-up-nca_fs_res_ca_all rsv.htm&amp;quot;);
[Test]
        public void Property_Address()
        {

            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET-42200.xls&quot;);
            Assert.AreEqual(workbook.Worksheets[0].Hyperlinks[0].Address, &quot;http://dev.dms.firstam.com/title/documents/work instructions/title/california/ca-res full search/full search write-up-nca_fs_res_ca_all rsv.htm&quot;);
        }
```

### See Also

* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


