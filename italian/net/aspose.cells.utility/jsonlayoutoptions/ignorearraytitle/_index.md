---
title: "JsonLayoutOptions.IgnoreArrayTitle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà JsonLayoutOptions. Indica se ignorare il titolo se l'array è una proprietà dell'oggetto"
type: docs
url: /it/net/aspose.cells.utility/jsonlayoutoptions/ignorearraytitle/
---
## JsonLayoutOptions.IgnoreArrayTitle property

Indica se ignorare il titolo se l'array è una proprietà dell'oggetto.

```csharp
[Obsolete("Use JsonLayoutOptions.IgnoreTitle property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IgnoreArrayTitle { get; set; }
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

    public class JsonLayoutOptionsPropertyIgnoreArrayTitleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Esempio di dati JSON con titoli di array
            string json = @"{
                ""Employees"": [
                    { ""Name"": ""John"", ""Age"": 30 },
                    { ""Name"": ""Jane"", ""Age"": 25 }
                ]
            }";

            // Crea JsonLayoutOptions
            JsonLayoutOptions options = new JsonLayoutOptions();
            
            // Visualizza il valore corrente di IgnoreArrayTitle
            Console.WriteLine("Current IgnoreArrayTitle value: " + options.IgnoreArrayTitle);

            // Prima importazione con IgnoreArrayTitle = false (predefinito)
            options.IgnoreArrayTitle = false;
            JsonUtility.ImportData(json, worksheet.Cells, 0, 0, options);
            Console.WriteLine("Data imported with IgnoreArrayTitle=false. Check cell A1 for 'Employees' title.");

            // Cancella il foglio di lavoro per la seconda importazione
            worksheet.Cells.Clear();

            // Seconda importazione con IgnoreArrayTitle = true
            options.IgnoreArrayTitle = true;
            JsonUtility.ImportData(json, worksheet.Cells, 0, 0, options);
            Console.WriteLine("Data imported with IgnoreArrayTitle=true. Check cell A1 for direct array values.");

            // Salva la cartella di lavoro
            workbook.Save("JsonLayoutOptionsIgnoreArrayTitleDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


