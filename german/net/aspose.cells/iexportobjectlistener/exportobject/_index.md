---
title: "IExportObjectListener.ExportObject"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "IExportObjectListener-Methode. Exportiere ein Objekt"
type: docs
url: /de/net/aspose.cells/iexportobjectlistener/exportobject/
---
## IExportObjectListener.ExportObject method

Exportiere ein Objekt.

```csharp
public object ExportObject(ExportObjectEvent e)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| e | ExportObjectEvent | Das Ereignis wird ausgelöst, wenn ein Objekt exportiert werden muss. |

### Rückgabewert

Die Informationen über das Ergebnis des Objektexports. Beim Exportieren von Objekten, wenn die Arbeitsmappe ins HTML-Format exportiert wird, ist das Ergebnis ein URL-String, um auf das gespeicherte Bild aus der HTML-Datei zuzugreifen, die dieses exportierte Objekt enthält.

### Beispiele

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

            // Ein Bild zum Arbeitsblatt hinzufügen
            int pictureIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[pictureIndex];

            // Erstellen Sie eine Instanz der Demo-Klasse, die IExportObjectListener implementiert
            var listener = new IExportObjectListenerMethodExportObjectWithExportObjectEventDemo();

            try
            {
                // In einem realen Szenario würde das ExportObjectEvent vom Framework bereitgestellt werden
                // Für Demonstrationszwecke rufen wir die Methode einfach mit null auf
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
            // Benutzerdefinierte Implementierung zur Handhabung des Exports
            if (e != null)
            {
                object source = e.GetSource();
                Console.WriteLine($"Exporting object of type: {source?.GetType().Name ?? "null"}");
            }
            else
            {
                Console.WriteLine("No export event provided (demo mode)");
            }

            // Geben Sie ein modifiziertes Objekt oder null zurück, um das Standard-Exportverhalten zu verwenden
            return null;
        }
    }
}
```

### Siehe auch

* class [ExportObjectEvent](../../exportobjectevent/)
* interface [IExportObjectListener](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


