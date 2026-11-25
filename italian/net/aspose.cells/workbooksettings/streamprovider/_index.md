---
title: "WorkbookSettings.StreamProvider"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookSettings. Ottiene e imposta il provider di flusso per risorse esterne"
type: docs
url: /it/net/aspose.cells/workbooksettings/streamprovider/
---
## WorkbookSettings.StreamProvider property

Ottiene e imposta il provider di flusso per la risorsa esterna.

```csharp
[Obsolete("Use ResourceProvider property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public IStreamProvider StreamProvider { get; set; }
```

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà ResourceProvider. Questa proprietà sarà rimossa 12 mesi dopo, a partire da giugno 2022. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class CustomStreamProvider1 : IStreamProvider
    {
        private MemoryStream stream;

        public void InitStream(StreamProviderOptions options)
        {
            stream = new MemoryStream();
            options.Stream = stream;
        }

        public void CloseStream(StreamProviderOptions options)
        {
            stream.Close();
            Console.WriteLine($"Stream closed. Content length: {stream.Length} bytes");
        }
    }

    public class WorkbookSettingsPropertyStreamProviderDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accedi alle impostazioni della cartella di lavoro
            WorkbookSettings settings = workbook.Settings;

            // Visualizza il valore corrente di StreamProvider
            Console.WriteLine("Current StreamProvider value: " + (settings.StreamProvider == null ? "null" : "custom provider"));

            // Imposta un provider di flusso personalizzato
            settings.StreamProvider = new CustomStreamProvider1();

            // Aggiungi alcuni dati per dimostrare l'uso del flusso
            worksheet.Cells["A1"].PutValue("Test data for stream provider");

            // Salva la cartella di lavoro - questo attiverà il provider di flusso
            workbook.Save("PropertyStreamProviderDemo.xlsx");

            // Reimposta il provider di flusso
            settings.StreamProvider = null;
            Console.WriteLine("StreamProvider reset to null");
        }
    }
}
```

### Vedi anche

* interface [IStreamProvider](../../istreamprovider/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


