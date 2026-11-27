---
title: "TxtLoadOptions.ExtendToNextSheet"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TxtLoadOptions-egenskap. Om data ska utökas till nästa blad när rader eller kolumner överskrider gränsen. Standard är false"
type: docs
url: /sv/net/aspose.cells/txtloadoptions/extendtonextsheet/
---
## TxtLoadOptions.ExtendToNextSheet property

Om data utökas till nästa blad när rader eller kolumner överskrider gränsen. Standard är falskt.

```csharp
public bool ExtendToNextSheet { get; set; }
```

### Anmärkningar

Om denna egenskap är true kommer extra data att placeras i nästa blad bakom det aktuella (om det aktuella bladet är det sista, kommer ett nytt blad att läggas till i den aktuella arbetsboken). Om denna egenskap är false kommer data som överskrider gränsen att ignoreras.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyExtendToNextSheetDemo
    {
        public static void Run()
        {
            // Skapa en exempel-CSV-sträng som överskrider vanliga kolumngränser i kalkylbladet
            string csvData = "A,B,C,D,E,F,G,H,I,J,K,L,M,N,O,P,Q,R,S,T,U,V,W,X,Y,Z,AA,AB,AC,AD,AE,AF,AG,AH,AI,AJ,AK,AL,AM,AN,AO,AP,AQ,AR,AS,AT,AU,AV,AW,AX,AY,AZ,BA,BB,BC,BD,BE,BF,BG,BH,BI,BJ,BK,BL,BM,BN,BO,BP,BQ,BR,BS,BT,BU,BV,BW,BX,BY,BZ,CA,CB,CC,CD,CE,CF,CG,CH,CI,CJ,CK,CL,CM,CN,CO,CP,CQ,CR,CS,CT,CU,CV,CW,CX,CY,CZ,DA,DB,DC,DD,DE,DF,DG,DH,DI,DJ,DK,DL,DM,DN,DO,DP,DQ,DR,DS,DT,DU,DV,DW,DX,DY,DZ,EA,EB,EC,ED,EE,EF,EG,EH,EI,EJ,EK,EL,EM,EN,EO,EP,EQ,ER,ES,ET,EU,EV,EW,EX,EY,EZ";

            // Skapa TxtLoadOptions med ExtendToNextSheet aktiverad
            TxtLoadOptions options = new TxtLoadOptions
            {
                ExtendToNextSheet = true
            };

            // Skapa en arbetsbok från CSV-data
            Workbook workbook = new Workbook(new MemoryStream(System.Text.Encoding.UTF8.GetBytes(csvData)), options);

            // Hämta cellerna från det första kalkylbladet
            Cells cells = workbook.Worksheets[0].Cells;

            // Skriv ut information om den importerade datan
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

### Se även

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


