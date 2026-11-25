---
title: "IFilePathProvider.GetFullName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo IFilePathProvider. Ottiene il percorso completo del file tramite il nome del foglio di lavoro quando si esporta il foglio di lavoro in HTML separatamente. In questo modo i riferimenti tra i fogli di lavoro possono essere esportati correttamente"
type: docs
url: /it/net/aspose.cells/ifilepathprovider/getfullname/
---
## IFilePathProvider.GetFullName method

Ottiene il percorso completo del file in base al nome del foglio di lavoro quando si esporta il foglio di lavoro in HTML separatamente. In questo modo i riferimenti tra i fogli di lavoro possono essere esportati correttamente.

```csharp
public string GetFullName(string sheetName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sheetName | String | Nome foglio di lavoro |

### Valore di ritorno

il percorso completo del file

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IFilePathProviderMethodGetFullNameWithStringDemo
    {
        public static void Run()
        {
            // Crea un'implementazione personalizzata di IFilePathProvider
            CustomFilePathProvider provider = new CustomFilePathProvider();

            // Chiama il metodo GetFullName con il nome di un foglio
            string sheetName = "Sheet1";
            string fullPath = provider.GetFullName(sheetName);

            // Visualizza il risultato
            Console.WriteLine($"Full path for {sheetName}: {fullPath}");
        }
    }

    internal class CustomFilePathProvider : IFilePathProvider
    {
        public string GetFullName(string sheetName)
        {
            // Implementazione semplice che restituisce un percorso combinando il nome del foglio con una directory
            return $"C:\\Temp\\{sheetName}.xlsx";
        }
    }
}
```

### Vedi anche

* interface [IFilePathProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


