---
title: "WorkbookSettings.StreamProvider"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings-egenskap. Hämtar och anger strömleverantören för extern resurs"
type: docs
url: /sv/net/aspose.cells/workbooksettings/streamprovider/
---
## WorkbookSettings.StreamProvider property

Hämtar och anger strömleverantören för extern resurs.

```csharp
[Obsolete("Use ResourceProvider property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public IStreamProvider StreamProvider { get; set; }
```

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället ResourceProvider-egenskapen. Denna egenskap kommer att tas bort 12 månader senare från och med juni 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Åtkomst till arbetsboksinställningar
            WorkbookSettings settings = workbook.Settings;

            // Visa aktuellt StreamProvider‑värde
            Console.WriteLine("Current StreamProvider value: " + (settings.StreamProvider == null ? "null" : "custom provider"));

            // Ange en anpassad strömleverantör
            settings.StreamProvider = new CustomStreamProvider1();

            // Lägg till lite data för att demonstrera strömanvändning
            worksheet.Cells["A1"].PutValue("Test data for stream provider");

            // Spara arbetsboken – detta kommer att utlösa strömleverantören
            workbook.Save("PropertyStreamProviderDemo.xlsx");

            // Återställ strömleverantören
            settings.StreamProvider = null;
            Console.WriteLine("StreamProvider reset to null");
        }
    }
}
```

### Se även

* interface [IStreamProvider](../../istreamprovider/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


