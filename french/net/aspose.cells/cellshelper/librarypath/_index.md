---
title: "CellsHelper.LibraryPath"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CellsHelper. Obtient ou définit le chemin de la bibliothèque qui est référencé par certaines références de formules externes"
type: docs
url: /fr/net/aspose.cells/cellshelper/librarypath/
---
## CellsHelper.LibraryPath property

Obtient ou définit le chemin de la bibliothèque qui est référencé par certaines références de formules externes.

```csharp
public static string LibraryPath { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperPropertyLibraryPathDemo
    {
        public static void Run()
        {
            // Définissez la propriété LibraryPath
            CellsHelper.LibraryPath = "C:\\MyLibraries\\AsposeCells";

            // Démontrez la récupération et l'utilisation de LibraryPath
            Console.WriteLine("Current Library Path: " + CellsHelper.LibraryPath);

            // Exemple d'utilisation du chemin dans une opération de fichier
            string filePath = System.IO.Path.Combine(CellsHelper.LibraryPath, "test.xlsx");
            Console.WriteLine("Would load file from: " + filePath);
        }
    }
}
```

### Voir aussi

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


