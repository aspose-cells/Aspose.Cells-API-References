---
title: "Cell.HasCustomFunction"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell property. Bu hücrenin formülünde özel işlevdesteklenmeyen işlevin olup olmadığını kontrol eder."
type: docs
url: /tr/net/aspose.cells/cell/hascustomfunction/
---
## Cell.HasCustomFunction property

Bu hücrenin formülünde özel bir işlev (desteklenmeyen işlev) olup olmadığını denetler.

```csharp
public bool HasCustomFunction { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyHasCustomFunctionDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook wb = new Workbook();
            
            // Özel bir işlev adı ekle
            NameCollection nc = wb.Worksheets.Names;
            nc[nc.Add("MyCustomFunc")].RefersTo = "=MYTESTFUNC()";
            
            // İlk çalışma sayfasına eriş
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Yerleşik işlevle test et
            Cell cell1 = cells[0, 0];
            cell1.Formula = "=SUM(A1:B1)";
            Console.WriteLine("HasCustomFunction (SUM): " + cell1.HasCustomFunction);
            
            // Özel işlevle test et
            Cell cell2 = cells[1, 0];
            cell2.Formula = "=MYTESTFUNC()";
            Console.WriteLine("HasCustomFunction (MYTESTFUNC): " + cell2.HasCustomFunction);
            
            // Özel işlev içeren adlandırılmış aralıkla test et
            Cell cell3 = cells[2, 0];
            cell3.Formula = "=MyCustomFunc";
            Console.WriteLine("HasCustomFunction (Named Range): " + cell3.HasCustomFunction);
            
            // İç içe özel işlevle test et
            Cell cell4 = cells[3, 0];
            cell4.Formula = "=SUM(MYTESTFUNC(), A1)";
            Console.WriteLine("HasCustomFunction (Nested): " + cell4.HasCustomFunction);
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


