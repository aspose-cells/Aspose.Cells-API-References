---
title: "Workbook.ProtectSharedWorkbook"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-metod. Skyddar en delad arbetsbok"
type: docs
url: /sv/net/aspose.cells/workbook/protectsharedworkbook/
---
## Workbook.ProtectSharedWorkbook method

Skyddar en delad arbetsbok.

```csharp
public void ProtectSharedWorkbook(string password)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| lösenord | String | Lösenord för att skydda workbooken. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodProtectSharedWorkbookWithStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook wb = new Workbook();
            
            // Skydda den delade arbetsboken med lösenord
            wb.ProtectSharedWorkbook("abcd");
            
            // Spara den skyddade arbetsboken
            wb.Save("ProtectedSharedWorkbook.xlsx");
            
            // Läs in den skyddade arbetsboken
            Workbook wbProtected = new Workbook("ProtectedSharedWorkbook.xlsx");
            
            // Verifiera skyddstatus
            Console.WriteLine("Workbook is protected: " + wbProtected.Settings.IsProtected);
            
            // Ta bort skyddet från workbook
            wbProtected.UnprotectSharedWorkbook("abcd");
            
            // Spara den oskyddade arbetsboken
            wbProtected.Save("UnprotectedSharedWorkbook.xlsx");
        }
    }
}
```

### Se även

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


