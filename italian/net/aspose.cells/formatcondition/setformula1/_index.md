---
title: "FormatCondition.SetFormula1"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "FormatCondition method. Imposta il valore o l'espressione associata a questa condizione di formattazione"
type: docs
url: /it/net/aspose.cells/formatcondition/setformula1/
---
## FormatCondition.SetFormula1 method

Imposta il valore o l'espressione associati a questa condizione di formato.

```csharp
public void SetFormula1(string formula, bool isR1C1, bool isLocal)
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

    public class FormatConditionMethodSetFormula1WithStringBooleanBooleanDemo
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

            // Aggiungi un intervallo di formattazione condizionale
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 3;
            area.EndColumn = 0;
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "30");

            // Ottieni la prima condizione di formattazione
            FormatCondition fc = fcc[0];

            try
            {
                // Chiama SetFormula1 con parametri (String, Boolean, Boolean)
                fc.SetFormula1("SUM(A1:A4)", false, false);

                // Visualizza il risultato
                Console.WriteLine("SetFormula1 executed successfully with formula: " + fc.Formula1);
                Console.WriteLine("Conditional formatting applied to range A1:A4 with formula: " + fc.Formula1);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetFormula1 method: {ex.Message}");
            }

            // Salva il risultato
            workbook.Save("FormatConditionSetFormula1Demo.xlsx");
        }
    }
}
```

### Vedi anche

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


