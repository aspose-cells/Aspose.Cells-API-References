---
title: "IconSet.Cfvos"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà IconSet. Ottieni l'istanza CFValueObjects"
type: docs
url: /it/net/aspose.cells/iconset/cfvos/
---
## IconSet.Cfvos property

Ottieni l'istanza CFValueObjects.

```csharp
public ConditionalFormattingValueCollection Cfvos { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IconSetPropertyCfvosDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i * 10);
            }

            try
            {
                // Aggiungi formattazione condizionale
                int cfIndex = worksheet.ConditionalFormattings.Add();
                FormatConditionCollection fcs = worksheet.ConditionalFormattings[cfIndex];

                // Imposta l'intervallo per la formattazione condizionale
                CellArea area = new CellArea();
                area.StartRow = 0;
                area.StartColumn = 0;
                area.EndRow = 9;
                area.EndColumn = 0;
                fcs.AddArea(area);

                // Aggiungi condizione al set di icone
                int conditionIndex = fcs.AddCondition(FormatConditionType.IconSet);
                FormatCondition condition = fcs[conditionIndex];

                // Imposta il tipo di set di icone
                condition.IconSet.Type = IconSetType.TrafficLights31;

                // Accedi alla proprietà Cfvos (sola lettura)
                ConditionalFormattingValueCollection cfvos = condition.IconSet.Cfvos;

                // Visualizza le informazioni sulla raccolta Cfvos
                Console.WriteLine("Number of CFValueObjects in the collection: " + cfvos.Count);

                // Itera attraverso la raccolta e visualizza ogni valore
                for (int i = 0; i < cfvos.Count; i++)
                {
                    ConditionalFormattingValue cfValue = cfvos[i];
                    Console.WriteLine($"CFValue {i + 1}: Type = {cfValue.Type}, Value = {cfValue.Value}");
                }

                // Salva la cartella di lavoro
                workbook.Save("IconSetCfvosDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with icon set conditional formatting.");
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

* class [ConditionalFormattingValueCollection](../../conditionalformattingvaluecollection/)
* class [IconSet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


