---
title: "Name.GetReferredAreas"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Name-Methode. Ruft alle von diesem Namen referenzierten Verweise ab"
type: docs
url: /de/net/aspose.cells/name/getreferredareas/
---
## Name.GetReferredAreas method

Liest alle Referenzen, auf die dieser Name verweist.

```csharp
public ReferredArea[] GetReferredAreas(bool recalculate)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| neu berechnen | Boolean | ob es neu berechnet wird, wenn dieser Name bereits vor diesem Aufruf berechnet wurde. |

### Rückgabewert

Alle Bereiche.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameMethodGetReferredAreasWithBooleanDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook wb = new Workbook();
            
            // Fügen Sie dem Arbeitsblatt einige Daten hinzu
            wb.Worksheets[0].Cells[3, 3].PutValue("v03");
            
            // Erstellen Sie einen benannten Bereich mit mehreren Verweisen
            Name n = wb.Worksheets.Names[wb.Worksheets.Names.Add("testname")];
            n.RefersTo = "='C:\\[extlink1.xlsx]Sheet1'!$A$1:$B$2,'C:\\[extlink2.xlsx]Sheet2'!$C$3,Sheet1!$D$4,'C:\\[extlink1.xlsx]Sheet1'!E5";
            
            // Rufen Sie referenzierte Bereiche mit externen Links ab
            ReferredArea[] ras = n.GetReferredAreas(true);
            
            // Zeigen Sie Informationen zu jedem referenzierten Bereich an
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
            
            // Erstellen Sie eine externe Arbeitsmappe und aktualisieren Sie Werte
            Workbook wb1 = new Workbook();
            wb1.Worksheets[0].Cells[0, 0].PutValue("v10");
            wb1.Worksheets[0].Cells[1, 1].PutValue("v11");
            wb1.Worksheets[0].Cells[4, 4].PutValue("v14");
            
            // Aktualisieren Sie die verknüpfte Datenquelle
            wb.UpdateLinkedDataSource(new Workbook[]{wb1});
            
            // Zeigen Sie einige Werte aus referenzierten Bereichen an
            Console.WriteLine("\nValues from referred areas:");
            Console.WriteLine($"Area1[0,0]: {ras[0].GetValue(0, 0)}");
            Console.WriteLine($"Area1[1,1]: {ras[0].GetValue(1, 1)}");
            Console.WriteLine($"Area3[0,0]: {ras[2].GetValue(0, 0)}");
            Console.WriteLine($"Area4[0,0]: {ras[3].GetValue(0, 0)}");
        }
    }
}
```

### Siehe auch

* class [ReferredArea](../../referredarea/)
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


