---
title: FindOptions.RegexKey
second_title: Aspose.Cells for .NET API Reference
description: FindOptions property. Indicates whether the searched key is regex. If true the searched key will be taken as regex and parsed. Otherwise the key will be parsed according to the rules in ms excel
type: docs
url: /net/aspose.cells/findoptions/regexkey/
---
## FindOptions.RegexKey property

Indicates whether the searched key is regex. If true the searched key will be taken as regex and parsed. Otherwise the key will be parsed according to the rules in ms excel.

```csharp
public bool RegexKey { get; set; }
```

### Remarks

Even though the search key has been specified as regex, it may be refactored according to specified [`LookAtType`](../lookattype/). For example, when the type is Contains(this is the default value for this options), wildcards will be added at the beginning and end of the search key automatically to ensure the match will be checked as "contains". In this case, the regular expressions will become more complex and the performance will also decrease. So, for performance consideration, if user has specified the exact rule for the regex, then there is no need to use [`LookAtType`](../lookattype/) as additional constraint and user may set it as EntireContent to get better performance.

### Examples

```csharp
// Called: options.RegexKey = true;
[Test]
        public void Property_RegexKey()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue("abc-123-xyz");
            workbook.Worksheets[0].Cells["E1"].PutValue("abc-123-xyz");
            FindOptions options = new FindOptions();
            options.RegexKey = true;
            Cell cell = workbook.Worksheets[0].Cells.Find("abc-*-xyz", null,null);
          Assert.AreEqual(cell.Name,"A1");
            cell = workbook.Worksheets[0].Cells.Find("abc-*-xyz", cell, null);
            Assert.AreEqual(cell.Name, "E1");
        }
```

### See Also

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


