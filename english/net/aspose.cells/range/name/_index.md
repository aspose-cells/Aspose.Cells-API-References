---
title: Range.Name
second_title: Aspose.Cells for .NET API Reference
description: Range property. Gets or sets the name of the range
type: docs
url: /net/aspose.cells/range/name/
---
## Range.Name property

Gets or sets the name of the range.

```csharp
public string Name { get; set; }
```

### Remarks

Named range is supported. For example,

range.Name = "Sheet1!MyRange";

### Examples

```csharp
// Called: str[i] = ranges[i * 10].Name;
[Test]
        public void Property_Name()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "Test_192442.xls");
            Aspose.Cells.Range[] ranges = workbook.Worksheets.GetNamedRanges();

            string[] str = new string[10];
            for (int i = 0; i < 10; i++)
            {
                str[i] = ranges[i * 10].Name;
            }
            workbook.Worksheets.Names.Remove(str);

            workbook.Save(Constants.destPath + "Test_192442.xls");
            workbook = new Workbook(Constants.destPath + "Test_192442.xls");
        }
```

### See Also

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


