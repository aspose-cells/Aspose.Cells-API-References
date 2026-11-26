---
title: "Clase FontSourceBase"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.FontSourceBase. Esta es una clase base abstracta para las clases que permiten al usuario especificar diversas fuentes tipográficas"
type: docs
url: /es/net/aspose.cells/fontsourcebase/
---
## FontSourceBase class

Esta es una clase base abstracta para las clases que permiten al usuario especificar diversas fuentes tipográficas

```csharp
public abstract class FontSourceBase
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| abstract [Type](../../aspose.cells/fontsourcebase/type/) { get; } | Devuelve el tipo del origen de la fuente. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassFontSourceBaseDemo
    {
        public static void Run()
        {
            // Crear una fuente tipográfica de carpeta
            string fontFolder = @"C:\Windows\Fonts";
            FolderFontSource folderSource = new FolderFontSource(fontFolder, true);

            // Mostrar propiedades de la fuente tipográfica
            Console.WriteLine($"Font folder: {folderSource.FolderPath}");
            Console.WriteLine($"Scan subfolders: {folderSource.ScanSubFolders}");
            Console.WriteLine($"Source type: {folderSource.Type}");

            // Crear libro de trabajo y establecer la fuente
            Workbook workbook = new Workbook();
            FontConfigs.SetFontSources(new FontSourceBase[] { folderSource });

            // Guardar con fuentes personalizadas
            workbook.Save("OutputWithCustomFonts.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


