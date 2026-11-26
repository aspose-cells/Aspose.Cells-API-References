---
title: "Clase FolderFontSource"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.FolderFontSource class. Representa la carpeta que contiene archivos de fuentes TrueType"
type: docs
url: /es/net/aspose.cells/folderfontsource/
---
## FolderFontSource class

Representa la carpeta que contiene archivos de fuentes TrueType.

```csharp
public class FolderFontSource : FontSourceBase
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [FolderFontSource](folderfontsource/)(string, bool) | Ctor. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [FolderPath](../../aspose.cells/folderfontsource/folderpath/) { get; } | Ruta a la carpeta de fuentes. |
| [ScanSubFolders](../../aspose.cells/folderfontsource/scansubfolders/) { get; } | Determina si escanear o no las subcarpetas. |
| override [Type](../../aspose.cells/folderfontsource/type/) { get; } | Devuelve el tipo del origen de la fuente. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FolderFontSourceDemo
    {
        public static void FolderFontSourceExample()
        {
            // Crear una instancia de FolderFontSource
            string folderPath = @"C:\Fonts";
            bool scanSubfolders = true;
            FolderFontSource folderFontSource = new FolderFontSource(folderPath, scanSubfolders);

            // Accediendo a propiedades
            Console.WriteLine("Folder Path: " + folderFontSource.FolderPath);
            Console.WriteLine("Scan Subfolders: " + folderFontSource.ScanSubFolders);
            Console.WriteLine("Font Source Type: " + folderFontSource.Type);

            // Crear un libro de trabajo y establecer los orígenes de fuentes
            Workbook workbook = new Workbook();
            FontConfigs.SetFontSources(new FontSourceBase[] { folderFontSource });

            // Guarda el libro de trabajo
            workbook.Save("FolderFontSourceExample.xlsx");
            workbook.Save("FolderFontSourceExample.pdf");
            return;
        }
    }
}
```

### Ver también

* class [FontSourceBase](../fontsourcebase/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


