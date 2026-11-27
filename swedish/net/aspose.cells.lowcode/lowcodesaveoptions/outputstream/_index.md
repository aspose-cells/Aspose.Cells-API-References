---
title: "LowCodeSaveOptions.OutputStream"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LowCodeSaveOptions egenskap. Hämtar och anger strömmen för att skriva den genererade datan till. När denna egenskap sätts till ett värde annat än null kommer OutputFile att ignoreras"
type: docs
url: /sv/net/aspose.cells.lowcode/lowcodesaveoptions/outputstream/
---
## LowCodeSaveOptions.OutputStream property

Hämtar och anger strömmen för att skriva den genererade datan till. När denna egenskap sätts till ett värde annat än null, kommer [`OutputFile`](../outputfile/) att ignoreras.

```csharp
public Stream OutputStream { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample OutputStream Demo");

            try
            {
                // Skapa LowCodeSaveOptions-instans
                LowCodeSaveOptions saveOptions = new LowCodeSaveOptions();
                
                // Skapa en minnesström för demonstration
                using (MemoryStream stream = new MemoryStream())
                {
                    // Ställ in OutputStream-egenskapen
                    saveOptions.OutputStream = stream;
                    saveOptions.SaveFormat = SaveFormat.Xlsx;

                    // Spara med hjälp av alternativen (kommer att skriva till vår minnesström)
                    workbook.Save(saveOptions.OutputStream, saveOptions.SaveFormat);

                    // Verifiera att strömmen skrevs till
                    Console.WriteLine($"OutputStream length: {saveOptions.OutputStream.Length} bytes");
                    Console.WriteLine("OutputStream position reset to 0 for reading");
                    saveOptions.OutputStream.Position = 0;

                    // Skapa en ny arbetsbok från strömmen för att verifiera innehållet
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

### Se även

* class [LowCodeSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


