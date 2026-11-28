---
title: "CellsHelper.LibraryPath"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CellsHelper özelliği. Bazı dış formül referansları tarafından başvurulan kütüphane yolunu alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/cellshelper/librarypath/
---
## CellsHelper.LibraryPath property

Bazı dış formül referansları tarafından kullanılan kütüphane yolunu alır veya ayarlar.

```csharp
public static string LibraryPath { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperPropertyLibraryPathDemo
    {
        public static void Run()
        {
            // LibraryPath özelliğini ayarla
            CellsHelper.LibraryPath = "C:\\MyLibraries\\AsposeCells";

            // LibraryPath'i almayı ve kullanmayı göster
            Console.WriteLine("Current Library Path: " + CellsHelper.LibraryPath);

            // Yolun bir dosya işleminde kullanılmasına örnek
            string filePath = System.IO.Path.Combine(CellsHelper.LibraryPath, "test.xlsx");
            Console.WriteLine("Would load file from: " + filePath);
        }
    }
}
```

### Ayrıca Bakınız

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


