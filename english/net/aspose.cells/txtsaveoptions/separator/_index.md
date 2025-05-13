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
// Called: txtSaveOptions.Separator = ',';
public void TxtSaveOptions_Property_Separator()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "TestWorkbook\\TestCellStyle_2.xls");
    TxtSaveOptions txtSaveOptions = new TxtSaveOptions();
    txtSaveOptions.Separator = ',';
    txtSaveOptions.Encoding = System.Text.Encoding.Unicode;
    workbook.Save(Constants.destPath + "example.csv", txtSaveOptions);
    FileStream fs = File.OpenRead(Constants.destPath + "example.csv");
    int firstByte = fs.ReadByte();
    int secondByte = fs.ReadByte();
    fs.Close();
    Assert.AreEqual((secondByte << 8) + firstByte, 0xFEFF);
    return;
}
```

### See Also

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


