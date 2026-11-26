---
title: "FolderFontSource.FolderFontSource"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor de FolderFontSource. Ctor"
type: docs
url: /es/net/aspose.cells/folderfontsource/folderfontsource/
---
## FolderFontSource constructor

Ctor.

```csharp
public FolderFontSource(string folderPath, bool scanSubfolders)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| folderPath | String | ruta a la carpeta de fuentes |
| scanSubfolders | Booleano | Determina si escanear o no subcarpetas. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FolderFontSourceMethodCtorWithStringBooleanDemo
    {
        public static void Run()
        {
            string folderPath = @"C:\Fonts";
            bool scanSubfolders = true;
            FolderFontSource folderFontSource = new FolderFontSource(folderPath, scanSubfolders);

            Console.WriteLine("Folder Path: " + folderFontSource.FolderPath);
            Console.WriteLine("Scan Subfolders: " + folderFontSource.ScanSubFolders);

            Workbook workbook = new Workbook();
            FontConfigs.SetFontSources(new FontSourceBase[] { folderFontSource });
            workbook.Save("FolderFontSourceExample.xlsx");
        }
    }
}
```

### Ver también

* class [FolderFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


