---
title: "FolderFontSource.FolderFontSource"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore di FolderFontSource. Ctor"
type: docs
url: /it/net/aspose.cells/folderfontsource/folderfontsource/
---
## FolderFontSource constructor

Ctor.

```csharp
public FolderFontSource(string folderPath, bool scanSubfolders)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| folderPath | String | percorso della cartella dei font |
| scanSubfolders | Booleano | Determina se scansionare o meno le sottocartelle. |

### Esempi

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

### Vedi anche

* class [FolderFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


