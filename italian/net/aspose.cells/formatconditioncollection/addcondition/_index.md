---
title: "FormatConditionCollection.AddCondition"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo FormatConditionCollection. Aggiunge una condizione di formattazione"
type: docs
url: /it/net/aspose.cells/formatconditioncollection/addcondition/
---
## AddCondition(FormatConditionType, OperatorType, string, string) {#addcondition_1}

Aggiunge una condizione di formattazione.

```csharp
public int AddCondition(FormatConditionType type, OperatorType operatorType, string formula1, 
    string formula2)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | FormatConditionType | Il tipo di condizione di formattazione. |
| operatorType | OperatorType | Il tipo di operatore |
| formula1 | String | Il valore o l'espressione associata alla formattazione condizionale. Se il valore di input inizia con '=', verrà considerato una formula. Altrimenti verrà considerato un valore semplice (testo, numero, bool). Per i valori di testo che iniziano con '=', l'utente può inserirlo come formula nel formato: \"=\\\"=...\\\"\". |
| formula2 | String | Il valore o l'espressione associata alla formattazione condizionale. Il formato di input è lo stesso di formula1 |

### Valore di ritorno

Indice dell'oggetto condizione di formattazione;

### Esempi

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionCollectionMethodAddConditionWithFormatConditionTypeOperatorTypDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];
            
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.EndRow = 10;
            ca.StartColumn = 0;
            ca.EndColumn = 10;
            fcs.AddArea(ca);
            
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "-50", "-1");
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.Font.Color = Color.Red;
            
            conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "0", "50");
            fc = fcs[conditionIndex];
            fc.Style.Font.Color = Color.Green;
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* enum [FormatConditionType](../../formatconditiontype/)
* enum [OperatorType](../../operatortype/)
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddCondition(FormatConditionType) {#addcondition}

Aggiungi una condizione di formattazione.

```csharp
public int AddCondition(FormatConditionType type)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | FormatConditionType | Tipo di condizione di formattazione. |

### Valore di ritorno

Indice dell'oggetto condizione di formattazione;

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionCollectionMethodAddConditionWithFormatConditionTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea condizioni di formattazione
            int formatIndex = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection conditions = worksheet.ConditionalFormattings[formatIndex];
            
            // Aggiungi intervallo
            CellArea area = new CellArea
            {
                StartRow = 0,
                StartColumn = 0,
                EndRow = 5,
                EndColumn = 5
            };
            conditions.AddArea(area);

            // Aggiungi condizioni (restituisce indice intero)
            conditions.AddCondition(FormatConditionType.ColorScale);
            conditions.AddCondition(FormatConditionType.IconSet);
            conditions.AddCondition(FormatConditionType.DataBar);

            workbook.Save("ConditionalFormattingDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [FormatConditionType](../../formatconditiontype/)
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


