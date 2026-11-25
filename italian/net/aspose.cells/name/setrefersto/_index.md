---
title: "Name.SetRefersTo"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Name. Imposta il riferimento di questo Name"
type: docs
url: /it/net/aspose.cells/name/setrefersto/
---
## Name.SetRefersTo method

Imposta il riferimento di questo Name.

```csharp
public void SetRefersTo(string refersTo, bool isR1C1, bool isLocal)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| refersTo | String | Il riferimento. |
| isR1C1 | Booleano | Indica se il riferimento è in formato R1C1. |
| isLocal | Booleano | Indica se il riferimento è formattato per la località. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class NameMethodSetRefersToWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati alle celle
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);

            // Crea un intervallo denominato
            int index = workbook.Worksheets.Names.Add("MyNamedRange");
            Name namedRange = workbook.Worksheets.Names[index];

            try
            {
                // Chiama SetRefersTo con parametri (String, Boolean, Boolean)
                namedRange.SetRefersTo("=Sheet1!$A$1:$A$3", false, false);

                // Visualizza il risultato
                Console.WriteLine($"Named range 'MyNamedRange' now refers to: {namedRange.RefersTo}");

                // Verifica utilizzando l'intervallo denominato in una formula
                worksheet.Cells["B1"].Formula = "=SUM(MyNamedRange)";
                workbook.CalculateFormula();

                Console.WriteLine($"Result of SUM(MyNamedRange): {worksheet.Cells["B1"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetRefersTo method: {ex.Message}");
            }

            // Salva la cartella di lavoro
            workbook.Save("NameMethodSetRefersToWithStringBooleanBooleanDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


