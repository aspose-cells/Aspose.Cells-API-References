---
title: "Name.GetReferredAreas"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Name-metod. Hämtar alla referenser som detta namn refererar till"
type: docs
url: /sv/net/aspose.cells/name/getreferredareas/
---
## Name.GetReferredAreas method

Hämtar alla referenser som refereras av detta namn.

```csharp
public ReferredArea[] GetReferredAreas(bool recalculate)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| omräkna | Boolean | om det ska omräknas om detta namn redan har beräknats före detta anrop. |

### Returvärde

Alla områden.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameMethodGetReferredAreasWithBooleanDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook wb = new Workbook();
            
            // Lägg till lite data i arbetsbladet
            wb.Worksheets[0].Cells[3, 3].PutValue("v03");
            
            // Skapa ett namngivet område med flera referenser
            Name n = wb.Worksheets.Names[wb.Worksheets.Names.Add("testname")];
            n.RefersTo = "='C:\\[extlink1.xlsx]Sheet1'!$A$1:$B$2,'C:\\[extlink2.xlsx]Sheet2'!$C$3,Sheet1!$D$4,'C:\\[extlink1.xlsx]Sheet1'!E5";
            
            // Hämta refererade områden med externa länkar
            ReferredArea[] ras = n.GetReferredAreas(true);
            
            // Visa information om varje refererat område
            Console.WriteLine("Number of referred areas: " + ras.Length);
            for (int i = 0; i < ras.Length; i++)
            {
                ReferredArea ra = ras[i];
                Console.WriteLine($"\nArea {i + 1}:");
                Console.WriteLine($"IsExternalLink: {ra.IsExternalLink}");
                if (ra.IsExternalLink)
                {
                    Console.WriteLine($"ExternalFileName: {ra.ExternalFileName}");
                }
                Console.WriteLine($"SheetName: {ra.SheetName}");
                Console.WriteLine($"IsArea: {ra.IsArea}");
                
                if (ra.IsArea)
                {
                    Console.WriteLine($"Range: {CellsHelper.CellIndexToName(ra.StartRow, ra.StartColumn)}" +
                                    $" to {CellsHelper.CellIndexToName(ra.EndRow, ra.EndColumn)}");
                }
                else
                {
                    Console.WriteLine($"Cell: {CellsHelper.CellIndexToName(ra.StartRow, ra.StartColumn)}");
                }
            }
            
            // Skapa en extern arbetsbok och uppdatera värden
            Workbook wb1 = new Workbook();
            wb1.Worksheets[0].Cells[0, 0].PutValue("v10");
            wb1.Worksheets[0].Cells[1, 1].PutValue("v11");
            wb1.Worksheets[0].Cells[4, 4].PutValue("v14");
            
            // Uppdatera länkad datakälla
            wb.UpdateLinkedDataSource(new Workbook[]{wb1});
            
            // Visa några värden från refererade områden
            Console.WriteLine("\nValues from referred areas:");
            Console.WriteLine($"Area1[0,0]: {ras[0].GetValue(0, 0)}");
            Console.WriteLine($"Area1[1,1]: {ras[0].GetValue(1, 1)}");
            Console.WriteLine($"Area3[0,0]: {ras[2].GetValue(0, 0)}");
            Console.WriteLine($"Area4[0,0]: {ras[3].GetValue(0, 0)}");
        }
    }
}
```

### Se även

* class [ReferredArea](../../referredarea/)
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


