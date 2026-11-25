---
title: "Enum FormatConditionValueType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.FormatConditionValueType. Tipo di valore della condizione"
type: docs
url: /it/net/aspose.cells/formatconditionvaluetype/
---
## FormatConditionValueType enumeration

Tipo di valore della condizione.

```csharp
public enum FormatConditionValueType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Formula | `0` | Il valore minimo/ medio / massimo per il gradiente è determinato da una formula. |
| Max | `1` | Indica che il valore massimo nell'intervallo deve essere usato come valore massimo per il gradiente. |
| Min | `2` | Indica che il valore minimo nell'intervallo deve essere usato come valore minimo per il gradiente. |
| Number | `3` | Indica che il valore minimo / medio / massimo per il gradiente è specificato da un valore numerico costante. |
| Percent | `4` | Il valore indica che una percentuale tra i valori minimo e massimo nell'intervallo deve essere usata come valore minimo / medio / massimo per il gradiente. |
| Percentile | `5` | Il valore indica che una classifica percentuale nell'intervallo deve essere usata come valore minimo / medio / massimo per il gradiente. |
| AutomaticMax | `6` | Indica che il valore massimo automatico nell'intervallo deve essere usato come valore massimo automatico per il gradiente. |
| AutomaticMin | `7` | Indica che il valore minimo automatico nell'intervallo deve essere usato come valore minimo automatico per il gradiente. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassFormatConditionValueTypeDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi condizioni di formattazione
            int formatConditionsIndex = sheet.ConditionalFormattings.Add();
            FormatConditionCollection formatConditions = sheet.ConditionalFormattings[formatConditionsIndex];
            int conditionIndex = formatConditions.AddCondition(FormatConditionType.IconSet);
            FormatCondition condition = formatConditions[conditionIndex];

            // Imposta le proprietà del set di icone
            condition.IconSet.Type = IconSetType.Boxes5;
            condition.IconSet.ShowValue = false;
            condition.IconSet.Reverse = true;

            // Imposta il valore della cella e applica la formattazione
            Cell cell = sheet.Cells["A1"];
            cell.PutValue("Boxes5 Icon Set Example");

            // Accedi al tipo di valore della condizione di formattazione
            FormatConditionValueType valueType = condition.IconSet.Cfvos[0].Type;
            Console.WriteLine("First CFVO Type: " + valueType);

            // Visualizza i valori dalle condizioni del set di icone
            Console.WriteLine("\nIcon Set Threshold Values:");
            foreach (ConditionalFormattingValue cfvo in condition.IconSet.Cfvos)
            {
                Console.WriteLine($"Type: {cfvo.Type}, Value: {cfvo.Value}");
            }

            // Salva la cartella di lavoro
            workbook.Save("FormatConditionValueTypeDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


