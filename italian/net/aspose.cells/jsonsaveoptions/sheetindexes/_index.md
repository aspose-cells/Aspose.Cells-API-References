---
title: "JsonSaveOptions.SheetIndexes"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà JsonSaveOptions. Rappresenta gli indici dei fogli esportati"
type: docs
url: /it/net/aspose.cells/jsonsaveoptions/sheetindexes/
---
## JsonSaveOptions.SheetIndexes property

Rappresenta gli indici dei fogli esportati.

```csharp
public int[] SheetIndexes { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class JsonSaveOptionsPropertySheetIndexesDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro con più fogli
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Popola alcuni dati in ogni foglio
            for (int i = 0; i < workbook.Worksheets.Count; i++)
            {
                Worksheet sheet = workbook.Worksheets[i];
                sheet.Cells["A1"].PutValue($"Data from Sheet {i + 1}");
            }

            // Crea un'istanza di JsonSaveOptions
            JsonSaveOptions options = new JsonSaveOptions();

            // Visualizza gli SheetIndexes correnti (null per impostazione predefinita - esporta tutti i fogli)
            Console.WriteLine("Current SheetIndexes: " + (options.SheetIndexes == null ? "Exporting all sheets" : string.Join(",", options.SheetIndexes)));

            // Imposta per esportare solo il primo e il terzo foglio (indici 0 e 2)
            options.SheetIndexes = new int[] { 0, 2 };

            // Salva in JSON con i fogli selezionati
            workbook.Save("JsonSaveOptionsPropertySheetIndexesDemo.json", options);

            // Verifica caricando il JSON
            string jsonContent = System.IO.File.ReadAllText("JsonSaveOptionsPropertySheetIndexesDemo.json");
            Console.WriteLine("JSON Content:");
            Console.WriteLine(jsonContent);

            // Modifica per esportare solo il secondo foglio (indice 1)
            options.SheetIndexes = new int[] { 1 };
            workbook.Save("JsonSaveOptionsPropertySheetIndexesDemo_SingleSheet.json", options);

            // Verifica l'esportazione di un singolo foglio
            jsonContent = System.IO.File.ReadAllText("JsonSaveOptionsPropertySheetIndexesDemo_SingleSheet.json");
            Console.WriteLine("Single Sheet JSON Content:");
            Console.WriteLine(jsonContent);
        }
    }
}
```

### Vedi anche

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


