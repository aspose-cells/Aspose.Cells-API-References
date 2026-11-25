---
title: "JsonLayoutOptions.IgnoreObjectTitle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà JsonLayoutOptions. Indica se ignorare il titolo se l'oggetto è una proprietà di un oggetto"
type: docs
url: /it/net/aspose.cells.utility/jsonlayoutoptions/ignoreobjecttitle/
---
## JsonLayoutOptions.IgnoreObjectTitle property

Indica se ignorare il titolo se l'oggetto è una proprietà di un oggetto.

```csharp
[Obsolete("Use JsonLayoutOptions.IgnoreTitle property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IgnoreObjectTitle { get; set; }
```

### Osservazioni

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà JsonLayoutOptions.IgnoreTitle. Questa proprietà sarà rimossa tra 6 mesi a partire da febbraio 2023. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Utility;
    using System;

    public class JsonLayoutOptionsPropertyIgnoreObjectTitleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Esempio di dati JSON con titoli degli oggetti
            string json = @"{
                ""Employees"": {
                    ""Employee"": [
                        { ""Name"": ""John"", ""Age"": 30 },
                        { ""Name"": ""Jane"", ""Age"": 25 }
                    ]
                }
            }";

            // Crea JsonLayoutOptions
            JsonLayoutOptions options = new JsonLayoutOptions();
            
            // Mostra il valore corrente di IgnoreObjectTitle
            Console.WriteLine("Current IgnoreObjectTitle value: " + options.IgnoreObjectTitle);

            // Imposta per ignorare i titoli degli oggetti
            options.IgnoreObjectTitle = true;
            Console.WriteLine("Set IgnoreObjectTitle to: " + options.IgnoreObjectTitle);

            // Importa JSON con IgnoreObjectTitle = true
            JsonUtility.ImportData(json, worksheet.Cells, 0, 0, options);

            // Salva con titoli ignorati
            workbook.Save("IgnoreObjectTitle_True.xlsx");

            // Reimposta il foglio di lavoro
            worksheet.Cells.Clear();

            // Imposta per includere i titoli degli oggetti
            options.IgnoreObjectTitle = false;
            Console.WriteLine("Set IgnoreObjectTitle to: " + options.IgnoreObjectTitle);

            // Importa JSON con IgnoreObjectTitle = false
            JsonUtility.ImportData(json, worksheet.Cells, 0, 0, options);

            // Salva con titoli inclusi
            workbook.Save("IgnoreObjectTitle_False.xlsx");
        }
    }
}
```

### Vedi anche

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


