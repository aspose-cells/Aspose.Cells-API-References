---
title: "TxtLoadOptions.ExtendToNextSheet"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TxtLoadOptions. Indica si extiende los datos a la siguiente hoja cuando las filas o columnas de datos superan el límite. El valor predeterminado es false"
type: docs
url: /es/net/aspose.cells/txtloadoptions/extendtonextsheet/
---
## TxtLoadOptions.ExtendToNextSheet property

Indica si extiende los datos a la siguiente hoja cuando las filas o columnas de datos superan el límite. El valor predeterminado es falso.

```csharp
public bool ExtendToNextSheet { get; set; }
```

### Observaciones

Si esta propiedad es true, los datos adicionales se colocarán en la siguiente hoja detrás de la actual (si la hoja actual es la última, se añadirá una nueva hoja al libro de trabajo). Si esta propiedad es false, los datos que superen el límite serán ignorados.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyExtendToNextSheetDemo
    {
        public static void Run()
        {
            // Cree una cadena CSV de muestra que exceda los límites normales de columnas de la hoja de cálculo
            string csvData = "A,B,C,D,E,F,G,H,I,J,K,L,M,N,O,P,Q,R,S,T,U,V,W,X,Y,Z,AA,AB,AC,AD,AE,AF,AG,AH,AI,AJ,AK,AL,AM,AN,AO,AP,AQ,AR,AS,AT,AU,AV,AW,AX,AY,AZ,BA,BB,BC,BD,BE,BF,BG,BH,BI,BJ,BK,BL,BM,BN,BO,BP,BQ,BR,BS,BT,BU,BV,BW,BX,BY,BZ,CA,CB,CC,CD,CE,CF,CG,CH,CI,CJ,CK,CL,CM,CN,CO,CP,CQ,CR,CS,CT,CU,CV,CW,CX,CY,CZ,DA,DB,DC,DD,DE,DF,DG,DH,DI,DJ,DK,DL,DM,DN,DO,DP,DQ,DR,DS,DT,DU,DV,DW,DX,DY,DZ,EA,EB,EC,ED,EE,EF,EG,EH,EI,EJ,EK,EL,EM,EN,EO,EP,EQ,ER,ES,ET,EU,EV,EW,EX,EY,EZ";

            // Cree TxtLoadOptions con ExtendToNextSheet habilitado
            TxtLoadOptions options = new TxtLoadOptions
            {
                ExtendToNextSheet = true
            };

            // Cree un libro de trabajo a partir de los datos CSV
            Workbook workbook = new Workbook(new MemoryStream(System.Text.Encoding.UTF8.GetBytes(csvData)), options);

            // Obtenga las celdas de la primera hoja de cálculo
            Cells cells = workbook.Worksheets[0].Cells;

            // Muestre información sobre los datos importados
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

### Ver también

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


