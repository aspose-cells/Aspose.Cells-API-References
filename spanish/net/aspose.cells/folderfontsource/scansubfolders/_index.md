---
title: "FolderFontSource.ScanSubFolders"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de FolderFontSource. Determina si escanear o no las subcarpetas"
type: docs
url: /es/net/aspose.cells/folderfontsource/scansubfolders/
---
## FolderFontSource.ScanSubFolders property

Determina si escanear o no las subcarpetas.

```csharp
public bool ScanSubFolders { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FolderFontSourcePropertyScanSubFoldersDemo
    {
        public static void Run()
        {
            // Crear una fuente de fuentes de carpeta con el escaneo de subcarpetas habilitado
            string folderPath = @"C:\Windows\Fonts"; // Typical system fonts folder
            bool scanSubfolders = true;
            FolderFontSource folderFontSource = new FolderFontSource(folderPath, scanSubfolders);

            // Mostrar propiedades de la fuente tipográfica
            Console.WriteLine("Folder Path: " + folderFontSource.FolderPath);
            Console.WriteLine("Scan Subfolders: " + folderFontSource.ScanSubFolders);

            // Crear un libro de trabajo y establecer la fuente de fuentes
            Workbook workbook = new Workbook();
            FontConfigs.SetFontSources(new FontSourceBase[] { folderFontSource });

            // Demostrar el uso estableciendo algún texto
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Text with fonts from folder source");

            // Guarda el libro de trabajo
            workbook.Save("FolderFontSourceDemo.xlsx");
        }
    }
}
```

### Ver también

* class [FolderFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


