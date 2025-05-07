---
title: Workbook.FileFormat
second_title: Aspose.Cells for .NET API Reference
description: Workbook property. Gets and sets the file format
type: docs
url: /net/aspose.cells/workbook/fileformat/
---
## Workbook.FileFormat property

Gets and sets the file format.

```csharp
public FileFormatType FileFormat { get; set; }
```

### Examples

```csharp
// Called: wb.Save(ms, GetSaveFormat(wb.FileFormat));
public static Workbook Property_FileFormat(string file)
        {
            using (MemoryStream ms = new MemoryStream(1048576))
            {
                Workbook wb = new Workbook(file);
                wb.Save(ms, GetSaveFormat(wb.FileFormat));
                ms.Position = 0;
                if (wb.FileFormat == FileFormatType.Csv)
                {
                    return new Workbook(ms, new TxtLoadOptions(LoadFormat.Csv));
                }
                if (wb.FileFormat == FileFormatType.Tsv)
                {
                    return new Workbook(ms, new TxtLoadOptions(LoadFormat.Tsv));
                }
                return new Workbook(ms);
            }
        }
```

### See Also

* enum [FileFormatType](../../fileformattype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


