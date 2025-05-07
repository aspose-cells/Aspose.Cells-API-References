---
title: LowCodeSaveOptions.OutputFile
second_title: Aspose.Cells for .NET API Reference
description: LowCodeSaveOptions property. Gets and sets the filewith path if needed for saving the generated data. When setting this property with value other than null or empty string OutputStream will be ignored
type: docs
url: /net/aspose.cells.lowcode/lowcodesaveoptions/outputfile/
---
## LowCodeSaveOptions.OutputFile property

Gets and sets the file(with path if needed) for saving the generated data. When setting this property with value other than null or empty string, [`OutputStream`](../outputstream/) will be ignored.

```csharp
public string OutputFile { get; set; }
```

### Examples

```csharp
// Called: OutputFile = Constants.checkPath + "License/LowCodeLock" + fnTail,
private void Property_OutputFile(Stream stream, string fnTail)
        {
            SpreadsheetLocker.Process(new LowCodeLoadOptions() { InputStream = stream },
                new LowCodeSaveOptions()
                {
                    OutputFile = Constants.checkPath + "License/LowCodeLock" + fnTail,
                }, "123456", "234567");
        }
```

### See Also

* class [LowCodeSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


