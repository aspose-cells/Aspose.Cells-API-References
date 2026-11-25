---
title: "CellsHelper.LibraryPath"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CellsHelper. Ottiene o imposta il percorso della libreria a cui si fa riferimento da alcune referenze di formule esterne"
type: docs
url: /it/net/aspose.cells/cellshelper/librarypath/
---
## CellsHelper.LibraryPath property

Ottiene o imposta il percorso della libreria a cui si fa riferimento da alcune formule esterne.

```csharp
public static string LibraryPath { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperPropertyLibraryPathDemo
    {
        public static void Run()
        {
            // Imposta la proprietà LibraryPath
            CellsHelper.LibraryPath = "C:\\MyLibraries\\AsposeCells";

            // Dimostra come ottenere e utilizzare LibraryPath
            Console.WriteLine("Current Library Path: " + CellsHelper.LibraryPath);

            // Esempio di utilizzo del percorso in un'operazione di file
            string filePath = System.IO.Path.Combine(CellsHelper.LibraryPath, "test.xlsx");
            Console.WriteLine("Would load file from: " + filePath);
        }
    }
}
```

### Vedi anche

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


