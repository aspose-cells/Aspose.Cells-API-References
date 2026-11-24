---
title: "TxtLoadOptions.ExtendToNextSheet"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TxtLoadOptions-Eigenschaft. Gibt an, ob Daten auf das nächste Blatt erweitert werden, wenn die Zeilen oder Spalten die Grenze überschreiten. Standard ist false"
type: docs
url: /de/net/aspose.cells/txtloadoptions/extendtonextsheet/
---
## TxtLoadOptions.ExtendToNextSheet property

Ob Daten auf das nächste Blatt erweitert werden, wenn die Zeilen oder Spalten die Grenze überschreiten. Standard ist false.

```csharp
public bool ExtendToNextSheet { get; set; }
```

### Hinweise

Wenn diese Eigenschaft true ist, werden zusätzliche Daten in das nächste Blatt hinter dem aktuellen Blatt eingefügt (wenn das aktuelle Blatt das letzte ist, wird ein neues Blatt zur aktuellen Arbeitsmappe hinzugefügt). Wenn diese Eigenschaft false ist, werden die die Grenze überschreitenden Daten ignoriert.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyExtendToNextSheetDemo
    {
        public static void Run()
        {
            // Erstelle einen Beispiel-CSV-String, der die normalen Spaltenlimits des Arbeitsblatts überschreitet
            string csvData = "A,B,C,D,E,F,G,H,I,J,K,L,M,N,O,P,Q,R,S,T,U,V,W,X,Y,Z,AA,AB,AC,AD,AE,AF,AG,AH,AI,AJ,AK,AL,AM,AN,AO,AP,AQ,AR,AS,AT,AU,AV,AW,AX,AY,AZ,BA,BB,BC,BD,BE,BF,BG,BH,BI,BJ,BK,BL,BM,BN,BO,BP,BQ,BR,BS,BT,BU,BV,BW,BX,BY,BZ,CA,CB,CC,CD,CE,CF,CG,CH,CI,CJ,CK,CL,CM,CN,CO,CP,CQ,CR,CS,CT,CU,CV,CW,CX,CY,CZ,DA,DB,DC,DD,DE,DF,DG,DH,DI,DJ,DK,DL,DM,DN,DO,DP,DQ,DR,DS,DT,DU,DV,DW,DX,DY,DZ,EA,EB,EC,ED,EE,EF,EG,EH,EI,EJ,EK,EL,EM,EN,EO,EP,EQ,ER,ES,ET,EU,EV,EW,EX,EY,EZ";

            // Erstelle TxtLoadOptions mit ExtendToNextSheet aktiviert
            TxtLoadOptions options = new TxtLoadOptions
            {
                ExtendToNextSheet = true
            };

            // Erstelle eine Arbeitsmappe aus den CSV-Daten
            Workbook workbook = new Workbook(new MemoryStream(System.Text.Encoding.UTF8.GetBytes(csvData)), options);

            // Hole die Zellen aus dem ersten Arbeitsblatt
            Cells cells = workbook.Worksheets[0].Cells;

            // Gib Informationen über die importierten Daten aus
            Console.WriteLine("Number of worksheets: " + workbook.Worksheets.Count);
            Console.WriteLine("Columns in first worksheet: " + workbook.Worksheets[0].Cells.MaxColumn);
            
            if (workbook.Worksheets.Count > 1)
            {
                Console.WriteLine("Columns in second worksheet: " + workbook.Worksheets[1].Cells.MaxColumn);
                Console.WriteLine("First cell in second worksheet: " + workbook.Worksheets[1].Cells[0, 0].StringValue);
            }
        }
    }
}
```

### Siehe auch

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


