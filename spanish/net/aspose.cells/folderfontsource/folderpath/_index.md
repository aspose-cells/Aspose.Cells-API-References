---
title: "FolderFontSource.FolderPath"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de FolderFontSource. Ruta a la carpeta de fuentes"
type: docs
url: /es/net/aspose.cells/folderfontsource/folderpath/
---
## FolderFontSource.FolderPath property

Ruta a la carpeta de fuentes.

```csharp
public string FolderPath { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FolderFontSourcePropertyFolderPathDemo
    {
        public static void Run()
        {
            // Crear una fuente tipográfica de carpeta
            string folderPath = @"C:\Windows\Fonts"; // Typical system fonts folder
            bool scanSubfolders = true;
            FolderFontSource folderFontSource = new FolderFontSource(folderPath, scanSubfolders);

            // Demostrar el uso de la propiedad FolderPath
            Console.WriteLine("Font folder path: " + folderFontSource.FolderPath);
            Console.WriteLine("Scan subfolders: " + folderFontSource.ScanSubFolders);

            // Crear libro de trabajo con la fuente de fuentes
            Workbook workbook = new Workbook();
            FontConfigs.SetFontSources(new FontSourceBase[] { folderFontSource });

            // Demostración simple - agregar texto que podría usar fuentes personalizadas
            workbook.Worksheets[0].Cells["A1"].PutValue("Font Source Demo");
            
            // Guardar salidas
            workbook.Save("FolderFontSourceDemo.xlsx");
        }
    }
}
```

### Ver también

* class [FolderFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


