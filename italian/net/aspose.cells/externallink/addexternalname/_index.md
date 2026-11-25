---
title: "ExternalLink.AddExternalName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ExternalLink. Aggiunge un nome esterno"
type: docs
url: /it/net/aspose.cells/externallink/addexternalname/
---
## ExternalLink.AddExternalName method

Aggiunge un nome esterno.

```csharp
public void AddExternalName(string text, string referTo)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| testo | String | Il testo del nome esterno. Se il nome esterno appartiene a un foglio di lavoro, il testo dovrebbe essere come Sheet1!Text. |
| referTo | String | Il referTo del nome esterno. Deve essere una cella o un intervallo. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkMethodAddExternalNameWithStringStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Crea una cartella di lavoro esterna di esempio
            Workbook externalWorkbook = new Workbook();
            Worksheet externalSheet = externalWorkbook.Worksheets[0];
            externalSheet.Cells["B2"].PutValue(67);
            
            // Aggiungi un collegamento esterno alla cartella di lavoro principale
            string[] sheetNames = new string[] { externalSheet.Name };
            int index = workbook.Worksheets.ExternalLinks.Add("ExternalWorkbook.xlsx", sheetNames);
            ExternalLink externalLink = workbook.Worksheets.ExternalLinks[index];
            
            // Aggiungi nome esterno
            externalLink.AddExternalName("Test", "=Sheet1!$B$2");
            
            // Usa il nome esterno in una formula
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].Formula = "=[ExternalWorkbook.xlsx]!Test";
            
            // Calcola la formula
            workbook.CalculateFormula();
            
            // Restituisci il risultato
            Console.WriteLine("Value from external reference: " + sheet.Cells["A1"].DoubleValue);
        }
    }
}
```

### Vedi anche

* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


