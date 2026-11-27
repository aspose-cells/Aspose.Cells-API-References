---
title: "Workbook.GetStyleInPool"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-metod. Hämtar stilen i stilpoolen. Alla stilar i workbook kommer att samlas i en pool. Det finns bara ett enkelt referensindex i cellerna."
type: docs
url: /sv/net/aspose.cells/workbook/getstyleinpool/
---
## Workbook.GetStyleInPool method

Hämtar stilen i stilpoolen. Alla stilar i arbetsboken kommer att samlas i en pool. Det finns bara ett enkelt referensindex i cellerna.

```csharp
public Style GetStyleInPool(int index)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | Int32 | Indexet. |

### Returvärde

Stilen i poolen motsvarar angivet index, kan vara null.

### Anmärkningar

Om den returnerade stilen ändras, kommer stilen för alla celler (som refererar till denna stil) att ändras.

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodGetStyleInPoolWithInt32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook wb = new Workbook();
            
            // Öppna första kalkylbladet och lägg till lite exempeldata
            Worksheet ws = wb.Worksheets[0];
            ws.Cells["A1"].PutValue("Sample Data");
            ws.Cells["A2"].PutValue(123.45);
            ws.Cells["A3"].PutValue(DateTime.Now);
            
            // Applicera några stilar
            Style style1 = wb.CreateStyle();
            style1.Custom = "$#,##0.00";
            ws.Cells["A2"].SetStyle(style1);
            
            Style style2 = wb.CreateStyle();
            style2.Custom = "yyyy-mm-dd";
            ws.Cells["A3"].SetStyle(style2);
            
            // Spara till minnesström
            using (MemoryStream ms = new MemoryStream())
            {
                wb.Save(ms, SaveFormat.Xlsx);
                
                // Läs in arbetsboken igen från strömmen
                ms.Position = 0;
                Workbook reloadWb = new Workbook(ms);
                
                // Hämta och visa stilar från stilpoolen
                int count = reloadWb.CountOfStylesInPool;
                Console.WriteLine($"Styles in pool: {count}");
                
                for (int i = 0; i < count; i++)
                {
                    Style style = reloadWb.GetStyleInPool(i);
                    Console.WriteLine($"Style {i}: CustomFormat={style.Custom}");
                }
            }
        }
    }
}
```

### Se även

* class [Style](../../style/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


