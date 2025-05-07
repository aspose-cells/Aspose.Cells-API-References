---
title: ReplaceOptions.CaseSensitive
second_title: Aspose.Cells for .NET API Reference
description: ReplaceOptions property. Indicates if the searched string is case sensitive
type: docs
url: /net/aspose.cells/replaceoptions/casesensitive/
---
## ReplaceOptions.CaseSensitive property

Indicates if the searched string is case sensitive.

```csharp
public bool CaseSensitive { get; set; }
```

### Examples

```csharp
// Called: options.CaseSensitive = false;
[Test]
        public void Property_CaseSensitive()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "Test_210499.xls");
            ReplaceOptions options = new ReplaceOptions();
            options.CaseSensitive = false;
            workbook.Replace("[b_officialname]", "Awesome Agency", options);
            Assert.AreEqual(workbook.Worksheets[0].Cells["A1"].StringValue, "Awesome Agency");
        }
```

### See Also

* class [ReplaceOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


