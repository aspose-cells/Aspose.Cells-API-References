---
title: "ConditionalFormattingValueCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ConditionalFormattingValueCollection. Ottieni l'elemento CFValueObject all'indice specificato"
type: docs
url: /it/net/aspose.cells/conditionalformattingvaluecollection/item/
---
## ConditionalFormattingValueCollection indexer

Ottieni l'elemento CFValueObject all'indice specificato.

```csharp
public ConditionalFormattingValue this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | L'indice a base zero dell'elemento. |

### Valore di ritorno

L'elemento all'indice specificato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ConditionalFormattingValueCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Aggiungi dati di esempio
                worksheet.Cells["A1"].PutValue(10);
                worksheet.Cells["A2"].PutValue(120);
                worksheet.Cells["A3"].PutValue(260);

                // Aggiungi formattazione condizionale
                int cfIndex = worksheet.ConditionalFormattings.Add();
                FormatConditionCollection fcs = worksheet.ConditionalFormattings[cfIndex];

                // Imposta l'intervallo per la formattazione condizionale
                CellArea ca = new CellArea
                {
                    StartRow = 0,
                    EndRow = 2,
                    StartColumn = 0,
                    EndColumn = 0
                };
                fcs.AddArea(ca);

                // Aggiungi una condizione di set di icone
                int conditionIndex = fcs.AddCondition(FormatConditionType.IconSet);
                FormatCondition condition = fcs[conditionIndex];
                IconSet iconSet = condition.IconSet;
                iconSet.Type = IconSetType.Arrows3;

                // Ottieni il ConditionalFormattingValueCollection
                ConditionalFormattingValueCollection cfvos = iconSet.Cfvos;

                // Aggiungi un valore alla collezione
                int valueIndex = cfvos.Add(FormatConditionValueType.Number, "50");

                // Dimostra l'accesso alla proprietà Item (indicizzatore)
                ConditionalFormattingValue cfv = cfvos[valueIndex];

                // Visualizza il valore dalla proprietà Item
                Console.WriteLine($"Conditional Formatting Value at index {valueIndex}:");
                Console.WriteLine($"  Type: {cfv.Type}");
                Console.WriteLine($"  Value: {cfv.Value}");
                Console.WriteLine($"  IsGTE: {cfv.IsGTE}");

                // Salva la cartella di lavoro
                workbook.Save("ConditionalFormattingValueCollectionItemDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [ConditionalFormattingValue](../../conditionalformattingvalue/)
* class [ConditionalFormattingValueCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


