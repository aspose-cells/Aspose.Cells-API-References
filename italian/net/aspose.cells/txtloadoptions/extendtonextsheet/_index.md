---
title: "TxtLoadOptions.ExtendToNextSheet"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TxtLoadOptions. Indica se estende i dati al foglio successivo quando le righe o le colonne dei dati superano il limite. Il valore predefinito è false"
type: docs
url: /it/net/aspose.cells/txtloadoptions/extendtonextsheet/
---
## TxtLoadOptions.ExtendToNextSheet property

Indica se estendere i dati al foglio successivo quando le righe o le colonne dei dati superano il limite. Il valore predefinito è false.

```csharp
public bool ExtendToNextSheet { get; set; }
```

### Osservazioni

Se questa proprietà è true, i dati extra verranno inseriti nel foglio successivo dietro a quello corrente (se il foglio corrente è l'ultimo, un nuovo foglio verrà aggiunto alla cartella di lavoro corrente). Se questa proprietà è false, i dati che superano il limite verranno ignorati.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyExtendToNextSheetDemo
    {
        public static void Run()
        {
            // Crea una stringa CSV di esempio che supera i limiti normali di colonne del foglio di lavoro
            string csvData = "A,B,C,D,E,F,G,H,I,J,K,L,M,N,O,P,Q,R,S,T,U,V,W,X,Y,Z,AA,AB,AC,AD,AE,AF,AG,AH,AI,AJ,AK,AL,AM,AN,AO,AP,AQ,AR,AS,AT,AU,AV,AW,AX,AY,AZ,BA,BB,BC,BD,BE,BF,BG,BH,BI,BJ,BK,BL,BM,BN,BO,BP,BQ,BR,BS,BT,BU,BV,BW,BX,BY,BZ,CA,CB,CC,CD,CE,CF,CG,CH,CI,CJ,CK,CL,CM,CN,CO,CP,CQ,CR,CS,CT,CU,CV,CW,CX,CY,CZ,DA,DB,DC,DD,DE,DF,DG,DH,DI,DJ,DK,DL,DM,DN,DO,DP,DQ,DR,DS,DT,DU,DV,DW,DX,DY,DZ,EA,EB,EC,ED,EE,EF,EG,EH,EI,EJ,EK,EL,EM,EN,EO,EP,EQ,ER,ES,ET,EU,EV,EW,EX,EY,EZ";

            // Crea TxtLoadOptions con ExtendToNextSheet abilitato
            TxtLoadOptions options = new TxtLoadOptions
            {
                ExtendToNextSheet = true
            };

            // Crea una cartella di lavoro dai dati CSV
            Workbook workbook = new Workbook(new MemoryStream(System.Text.Encoding.UTF8.GetBytes(csvData)), options);

            // Ottieni le celle dal primo foglio di lavoro
            Cells cells = workbook.Worksheets[0].Cells;

            // Emetti informazioni sui dati importati
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

### Vedi anche

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


