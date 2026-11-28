---
title: "PasteOptions.KeepOldTables"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PasteOptions özelliği. Hedef aralıktaki tabloları korur"
type: docs
url: /tr/net/aspose.cells/pasteoptions/keepoldtables/
---
## PasteOptions.KeepOldTables property

Tabloları hedef aralıkta tutar.

```csharp
public bool KeepOldTables { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PasteOptionsPropertyKeepOldTablesDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Veri içeren örnek bir çalışma sayfası oluştur
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Source Data";
            worksheet.Cells["B1"].Value = "Table Data";

            try
            {
                // Bir PasteOptions örneği oluştur
                PasteOptions pasteOptions = new PasteOptions();

                // KeepOldTables özelliğinin varsayılan değerini göster
                Console.WriteLine("Default KeepOldTables value: " + pasteOptions.KeepOldTables);

                // KeepOldTables değerini true olarak ayarla
                pasteOptions.KeepOldTables = true;
                Console.WriteLine("KeepOldTables set to: " + pasteOptions.KeepOldTables);

                // Kopyalama işlemi için aralıklar oluştur
                Aspose.Cells.Range sourceRange = worksheet.Cells.CreateRange("A1:B1");
                Aspose.Cells.Range targetRange = worksheet.Cells.CreateRange("A3:B3");

                // KeepOldTables seçeneğiyle kopyala
                targetRange.Copy(sourceRange, pasteOptions);

                // Çalışma kitabını kaydedin
                workbook.Save("KeepOldTablesDemo.xlsx");
                Console.WriteLine("Workbook saved with KeepOldTables option applied.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


