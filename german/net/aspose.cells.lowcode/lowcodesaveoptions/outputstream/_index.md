---
title: "LowCodeSaveOptions.OutputStream"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LowCodeSaveOptions-Eigenschaft. Gibt den Stream zum Schreiben der erzeugten Daten zurück und legt ihn fest. Beim Setzen dieser Eigenschaft mit einem Wert ungleich null wird OutputFile ignoriert"
type: docs
url: /de/net/aspose.cells.lowcode/lowcodesaveoptions/outputstream/
---
## LowCodeSaveOptions.OutputStream property

Gibt den Stream zum Schreiben der erzeugten Daten zurück und legt ihn fest. Beim Setzen dieser Eigenschaft mit einem Wert ungleich null wird [`OutputFile`](../outputfile/) ignoriert.

```csharp
public Stream OutputStream { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;
    using System.IO;

    public class LowCodeSaveOptionsPropertyOutputStreamDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample OutputStream Demo");

            try
            {
                // Erstelle eine LowCodeSaveOptions-Instanz
                LowCodeSaveOptions saveOptions = new LowCodeSaveOptions();
                
                // Erstelle einen Memory-Stream zur Demonstration
                using (MemoryStream stream = new MemoryStream())
                {
                    // Setze die OutputStream-Eigenschaft
                    saveOptions.OutputStream = stream;
                    saveOptions.SaveFormat = SaveFormat.Xlsx;

                    // Speichere mit den Optionen (wird in unseren Memory-Stream schreiben)
                    workbook.Save(saveOptions.OutputStream, saveOptions.SaveFormat);

                    // Überprüfe, ob in den Stream geschrieben wurde
                    Console.WriteLine($"OutputStream length: {saveOptions.OutputStream.Length} bytes");
                    Console.WriteLine("OutputStream position reset to 0 for reading");
                    saveOptions.OutputStream.Position = 0;

                    // Erstelle ein neues Workbook aus dem Stream, um den Inhalt zu überprüfen
                    Workbook verifyWorkbook = new Workbook(saveOptions.OutputStream);
                    Console.WriteLine($"Verified worksheet count: {verifyWorkbook.Worksheets.Count}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [LowCodeSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


