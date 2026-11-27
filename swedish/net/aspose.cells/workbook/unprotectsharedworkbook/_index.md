---
title: "Workbook.UnprotectSharedWorkbook"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-metod. Låser upp en delad arbetsbok"
type: docs
url: /sv/net/aspose.cells/workbook/unprotectsharedworkbook/
---
## Workbook.UnprotectSharedWorkbook method

Avskyddar en delad arbetsbok.

```csharp
public void UnprotectSharedWorkbook(string password)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| lösenord | String | Lösenord för att låsa upp arbetsboken. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodUnprotectSharedWorkbookWithStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook wb = new Workbook();
            
            // Skydda den delade arbetsboken med lösenord
            wb.ProtectSharedWorkbook("abcd");
            
            // Spara den skyddade arbetsboken
            wb.Save("ProtectedSharedWorkbook.xlsx");
            
            // Öppna arbetsboken igen
            wb = new Workbook("ProtectedSharedWorkbook.xlsx");
            
            // Lås upp den delade arbetsboken med lösenord
            wb.UnprotectSharedWorkbook("abcd");
            
            // Spara den oskyddade arbetsboken
            wb.Save("UnprotectedSharedWorkbook.xlsx");
        }
    }
}
```

### Se även

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


