---
title: Workbook.HasMacro
second_title: Aspose.Cells for .NET API Reference
description: Workbook property. Indicates if this spreadsheet contains macro/VBA
type: docs
url: /net/aspose.cells/workbook/hasmacro/
---
## Workbook.HasMacro property

Indicates if this spreadsheet contains macro/VBA.

```csharp
public bool HasMacro { get; }
```

### Examples

```csharp
// Called: Assert.IsFalse(workbook.HasMacro);
[Test]
        public void Property_HasMacro()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSJAVA42658.xlsm");
            Assert.AreEqual(workbook.FileFormat,FileFormatType.Xlsm);
            Assert.IsTrue(workbook.HasMacro);
            workbook.Save(Constants.destPath + "CELLSJAVA42658.xlsm");
            workbook = new Workbook(Constants.destPath + "CELLSJAVA42658.xlsm");
            Assert.AreEqual(workbook.FileFormat, FileFormatType.Xlsm);
            Assert.IsTrue(workbook.HasMacro);
            workbook.Save(Constants.destPath + "CELLSJAVA42658.xlsx");
            workbook = new Workbook(Constants.destPath + "CELLSJAVA42658.xlsx");
            Assert.AreEqual(workbook.FileFormat, FileFormatType.Xlsx);
            Assert.IsFalse(workbook.HasMacro);
            Assert.AreEqual(SheetType.Worksheet, workbook.Worksheets[3].Type);
        }
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


