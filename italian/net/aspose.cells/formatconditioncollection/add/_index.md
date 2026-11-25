---
title: "FormatConditionCollection.Add"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo FormatConditionCollection. Aggiunge una condizione di formattazione e l'intervallo di celle interessato alle FormatConditions. Le FormatConditions possono contenere fino a tre formati condizionali. I riferimenti ad altri fogli non sono consentiti nelle formule della formattazione condizionale"
type: docs
url: /it/net/aspose.cells/formatconditioncollection/add/
---
## FormatConditionCollection.Add method

Aggiunge una condizione di formattazione e l'intervallo di celle interessato alle FormatConditions. Le FormatConditions possono contenere fino a tre formati condizionali. I riferimenti ad altri fogli non sono consentiti nelle formule della formattazione condizionale.

```csharp
public int[] Add(CellArea cellArea, FormatConditionType type, OperatorType operatorType, 
    string formula1, string formula2)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cellArea | CellArea | Intervallo di celle formattato condizionalmente. |
| type | FormatConditionType | Tipo di formattazione condizionale.Potrebbe essere uno dei membri di FormatConditionType. |
| operatorType | OperatorType | Operatore di confronto.Potrebbe essere uno dei membri di OperatorType. |
| formula1 | String | Il valore o l'espressione associata alla formattazione condizionale. |
| formula2 | String | Il valore o l'espressione associata alla formattazione condizionale |

### Valore di ritorno

[0]:Formatting condition object index;[1] Effected cell rang index.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionCollectionMethodAddWithCellAreaFormatConditionTypeOpeDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Popola dati di esempio
            for (int i = 0; i < 5; i++)
            {
                cells[i, 0].PutValue(i);
            }

            // Aggiungi formattazione condizionale
            ConditionalFormattingCollection cfc = sheet.ConditionalFormattings;
            FormatConditionCollection fcc = cfc[cfc.Add()];
            
            // Dimostrare il metodo Add con parametri specificati
            fcc.Add(
                CellArea.CreateCellArea(0, 0, 4, 0),
                FormatConditionType.Expression,
                OperatorType.None,
                "=A1>AVERAGE(OFFSET($A$1:$A$5,0,0)-0)",
                null
            );

            // Applicare la formattazione
            int fontSize = wb.DefaultStyle.Font.Size;
            fcc[0].Style.Font.Size = fontSize + 2;

            // Salvare la cartella di lavoro per dimostrare il risultato
            wb.Save("ConditionalFormattingDemo.xlsx");
        }
    }
}
```

### Vedi anche

* struct [CellArea](../../cellarea/)
* enum [FormatConditionType](../../formatconditiontype/)
* enum [OperatorType](../../operatortype/)
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


