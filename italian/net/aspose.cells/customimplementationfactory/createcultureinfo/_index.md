---
title: "CustomImplementationFactory.CreateCultureInfo"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo CustomImplementationFactory. Crea un oggetto CultureInfo con l'ID fornito"
type: docs
url: /it/net/aspose.cells/customimplementationfactory/createcultureinfo/
---
## CustomImplementationFactory.CreateCultureInfo method

Crea un oggetto CultureInfo con l'ID fornito.

```csharp
public virtual CultureInfo CreateCultureInfo(int lcid)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| lcid | Int32 |  |

### Valore di ritorno

L'istanza di CultureInfo.

### Osservazioni

Questa implementazione è utile per le seguenti situazioni: 1. Alcune culture potrebbero non essere supportate dall'ambiente dell'utente e la creazione del CultureInfo richiesto con l'identificatore fornito potrebbe generare un'Exception. Per evitare l'eccezione, l'utente può sovrascrivere questo metodo per fornire un'istanza di CultureInfo valida per quella non supportata. 2. L'utente potrebbe voler specificare alcune proprietà personalizzate per alcune culture per ottenere il risultato previsto nella formattazione. A tal fine l'utente può sovrascrivere questo metodo per fornire l'istanza di CultureInfo con le proprietà specificate dall'utente. Si noti che la proprietà UseUserOverride dell'istanza di CultureInfo restituita può influenzare il risultato formattato. Se è false, alcune proprietà dell'istanza di CultureInfo restituita possono essere sovrascritte dal nostro motore di formattazione integrato in base ai requisiti di formattazione di diversi scenari. Se è true, non modificheremo alcuna proprietà e la utilizzeremo per formattare i valori direttamente. Pertanto, se l'utente ha specificato proprietà personalizzate per l'istanza di CultureInfo restituita, assicurarsi che UseUserOverride sia true.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Globalization;

    public class CustomImplementationFactoryMethodCreateCultureInfoWithInt32Demo
    {
        public static void Run()
        {
            try
            {
                // Crea un'istanza di CustomImplementationFactory
                CustomImplementationFactory factory = new CustomImplementationFactory();

                // Chiama CreateCultureInfo con un LCID valido (1033 per English - United States)
                int lcid = 1033;
                CultureInfo cultureInfo = factory.CreateCultureInfo(lcid);

                // Visualizza i risultati
                Console.WriteLine($"CultureInfo created successfully with LCID: {lcid}");
                Console.WriteLine($"Culture Name: {cultureInfo.Name}");
                Console.WriteLine($"Display Name: {cultureInfo.DisplayName}");
                Console.WriteLine($"English Name: {cultureInfo.EnglishName}");

                // Dimostra l'impostazione della factory in CellsHelper
                CellsHelper.CustomImplementationFactory = factory;
                Console.WriteLine("CustomImplementationFactory set in CellsHelper.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling CreateCultureInfo: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [CustomImplementationFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


