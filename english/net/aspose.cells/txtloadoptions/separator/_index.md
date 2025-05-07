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
// Called: txtLoadOption.Separator = ';';
[Test, Category("Bug")]
        public void Property_Separator()
        {
            Workbook workbook = new Workbook();
            TxtLoadOptions txtLoadOption = new TxtLoadOptions();
            txtLoadOption.Separator = ';';
            //workbook.Open(Constants.sourcePath +"TestCells16011.csv", ';');
            workbook = new Workbook(Constants.sourcePath + "TestCells16011.csv", txtLoadOption);
        }
```

### See Also

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


