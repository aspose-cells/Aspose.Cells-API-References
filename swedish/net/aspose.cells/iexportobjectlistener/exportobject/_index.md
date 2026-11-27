---
title: "IExportObjectListener.ExportObject"
second_title: "Aspose.Cells för .NET API‑referens"
description: "IExportObjectListener metod. Exportera ett objekt"
type: docs
url: /sv/net/aspose.cells/iexportobjectlistener/exportobject/
---
## IExportObjectListener.ExportObject method

Exportera ett objekt.

```csharp
public object ExportObject(ExportObjectEvent e)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| e | ExportObjectEvent | Händelsen som utlöses när ett objekt behöver exporteras. |

### Returvärde

Informationen om resultatet av att exportera objektet. Vid export av objekt när arbetsboken exporteras till HTML-format är resultatet en URL‑sträng för att komma åt den sparade bilden från HTML‑filen som innehåller detta exporterade objekt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class IExportObjectListenerMethodExportObjectWithExportObjectEventDemo : IExportObjectListener
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en bild i arbetsbladet
            int pictureIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[pictureIndex];

            // Skapa en instans av demoklassen som implementerar IExportObjectListener
            var listener = new IExportObjectListenerMethodExportObjectWithExportObjectEventDemo();

            try
            {
                // I ett riktigt scenario skulle ExportObjectEvent tillhandahållas av ramverket
                // För demonstrationsändamål kommer vi bara att anropa metoden med null
                object result = listener.ExportObject(null);

                Console.WriteLine("ExportObject method executed successfully.");
                Console.WriteLine($"Returned object type: {result?.GetType().Name ?? "null"}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ExportObject method: {ex.Message}");
            }

            workbook.Save("ExportObjectDemo.xlsx");
        }

        public object ExportObject(ExportObjectEvent e)
        {
            // Anpassad implementation för att hantera exporten
            if (e != null)
            {
                object source = e.GetSource();
                Console.WriteLine($"Exporting object of type: {source?.GetType().Name ?? "null"}");
            }
            else
            {
                Console.WriteLine("No export event provided (demo mode)");
            }

            // Returnera ett modifierat objekt eller null för att använda standardexportbeteende
            return null;
        }
    }
}
```

### Se även

* class [ExportObjectEvent](../../exportobjectevent/)
* interface [IExportObjectListener](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


