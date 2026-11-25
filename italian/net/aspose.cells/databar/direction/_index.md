---
title: "DataBar.Direction"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DataBar. Ottiene o imposta la direzione in cui la barra dati è visualizzata"
type: docs
url: /it/net/aspose.cells/databar/direction/
---
## DataBar.Direction property

Ottiene o imposta la direzione in cui viene visualizzata la DataBar.

```csharp
public TextDirectionType Direction { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DataBarPropertyDirectionDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per dimostrare le barre dei dati
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].Value = i + 1;  // Values from 1 to 10 in column A
            }

            // Aggiungi formattazione condizionale della barra dati
            ConditionalFormattingCollection conditionalFormattings = worksheet.ConditionalFormattings;
            int index = conditionalFormattings.Add();
            FormatConditionCollection conditionalFormatting = conditionalFormattings[index];
            
            // Definisci l'area della cella per la condizione di formattazione
            CellArea cellArea = new CellArea
            {
                StartRow = 0,
                StartColumn = 0,
                EndRow = 9,
                EndColumn = 0
            };
            conditionalFormatting.AddArea(cellArea);

            // Aggiungi la condizione DataBar e ottieni il riferimento
            int conditionIndex = conditionalFormatting.AddCondition(FormatConditionType.DataBar);
            FormatCondition condition = conditionalFormatting[conditionIndex];

            DataBar dataBar = condition.DataBar;

            // Visualizza il valore corrente di Direction
            Console.WriteLine("Initial DataBar Direction: " + dataBar.Direction);

            // Cambia la direzione a RightToLeft e dimostra
            dataBar.Direction = TextDirectionType.RightToLeft;

            // Configurazione aggiuntiva per una migliore visualizzazione
            dataBar.Color = System.Drawing.Color.LightGreen;
            dataBar.MinCfvo.Type = FormatConditionValueType.Min;
            dataBar.MaxCfvo.Type = FormatConditionValueType.Max;

            // Salva la cartella di lavoro per mostrare l'effetto
            workbook.Save("DataBarDirectionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [TextDirectionType](../../textdirectiontype/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


