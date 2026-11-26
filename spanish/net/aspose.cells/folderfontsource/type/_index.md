---
title: "FolderFontSource.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de FolderFontSource. Devuelve el tipo de la fuente de fuentes"
type: docs
url: /es/net/aspose.cells/folderfontsource/type/
---
## FolderFontSource.Type property

Devuelve el tipo del origen de la fuente.

```csharp
public override FontSourceType Type { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FolderFontSourcePropertyTypeDemo
    {
        public static void Run()
        {
            string folderPath = @"C:\Fonts";
            bool scanSubfolders = true;
            FolderFontSource folderFontSource = new FolderFontSource(folderPath, scanSubfolders);

            Console.WriteLine("Folder Path: " + folderFontSource.FolderPath);
            Console.WriteLine("Scan Subfolders: " + folderFontSource.ScanSubFolders);
            Console.WriteLine("Font Source Type: " + folderFontSource.Type);

            Workbook workbook = new Workbook();
            FontConfigs.SetFontSources(new FontSourceBase[] { folderFontSource });

            workbook.Save("FolderFontSourceExample.xlsx");
        }
    }
}
```

### Ver también

* enum [FontSourceType](../../fontsourcetype/)
* class [FolderFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


