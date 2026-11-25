---
title: "FormatCondition.SetFormula2"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "FormatCondition method. Imposta il valore o l'espressione associata a questa condizione di formattazione"
type: docs
url: /it/net/aspose.cells/formatcondition/setformula2/
---
## FormatCondition.SetFormula2 method

Imposta il valore o l'espressione associati a questa condizione di formato.

```csharp
public void SetFormula2(string formula, bool isR1C1, bool isLocal)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| formula | String | Il valore o l'espressione associata a questa condizione di formattazione. Se il valore di input inizia con '=', verrà considerato una formula. Altrimenti verrà considerato un valore semplice (testo, numero, bool). Per i valori di testo che iniziano con '=', l'utente può inserirlo come formula nel formato: "=\"=...\"". |
| isR1C1 | Booleano | Indica se la formula è una formula R1C1. |
| isLocal | Booleano | Se la formula è formattata secondo la locale. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FormatConditionMethodSetFormula2WithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // Aggiungi una condizione di formattazione
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 3;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "30");

            // Ottieni la prima condizione di formattazione
            FormatCondition fc = fcs[0];

            try
            {
                // Chiama SetFormula2 con i parametri (String, Boolean, Boolean)
                fc.SetFormula2("25", false, false);

                // Visualizza il risultato
                Console.WriteLine("SetFormula2 executed successfully. New Formula2: " + fc.Formula2);
                Console.WriteLine("Cells A1:A4 will be formatted if their values are between 10 and 25");

                // Applica uno stile per rendere visibile l'effetto
                Style style = workbook.CreateStyle();
                style.BackgroundColor = System.Drawing.Color.LightGreen;
                fc.Style = style;
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetFormula2 method: {ex.Message}");
            }

            // Salva il risultato
            workbook.Save("FormatConditionSetFormula2Demo.xlsx");
        }
    }
}
```

### Vedi anche

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


