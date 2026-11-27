---
title: "PclSaveOptions.EmbedFont"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PclSaveOptions-egenskapen. Anger om teckensnittet ska bäddas in i den utgående Pcl-filen."
type: docs
url: /sv/net/aspose.cells/pclsaveoptions/embedfont/
---
## PclSaveOptions.EmbedFont property

Anger om teckensnitt ska bäddas in i den genererade Pcl-filen.

```csharp
public bool EmbedFont { get; set; }
```

### Anmärkningar

Standardvärdet är sant.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PclSaveOptionsPropertyEmbedFontDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och lägg till några exempeldata
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Demonstrating EmbedFont property");
            sheet.Cells["A2"].PutValue(DateTime.Now);

            try
            {
                // Skapa PCL‑spara‑alternativ
                PclSaveOptions pclOptions = new PclSaveOptions();

                // Läs och visa det aktuella värdet för EmbedFont-egenskapen.
                Console.WriteLine("Current EmbedFont value: " + pclOptions.EmbedFont);

                // (Valfritt) Om egenskapen är skrivbar kan du sätta den, men vi läser bara den här.
                // pclOptions.EmbedFont = true;

                // Spara arbetsboken som en PCL-fil med hjälp av alternativen.
                workbook.Save("EmbedFontDemo.pcl", pclOptions);

                Console.WriteLine("Workbook saved successfully with EmbedFont demonstration.");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error: " + ex.Message);
            }
        }
    }
}
```

### Se även

* class [PclSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


