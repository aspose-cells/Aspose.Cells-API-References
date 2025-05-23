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
public void FindOptions_Property_RegexKey()
{
    string filePath = Constants.sourcePath + "example.xlsx";
    string testStr = "[hello], [list3], [another_example]. However";
    string regEx = "\\[[a-zA-Z0-9_]+]";
    Workbook workbook = new Workbook(filePath);
    Worksheet worksheet = workbook.Worksheets[0];
    FindOptions options = new FindOptions();
    options.RegexKey = true;
    options.LookInType = LookInType.Values;
    options.LookAtType = LookAtType.Contains;
    //Cells.Find method does not find any cell with regEx
    Cell found = worksheet.Cells.Find(regEx, null, options);
    Assert.AreEqual(found.Name, "A1");
}
```

### See Also

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


