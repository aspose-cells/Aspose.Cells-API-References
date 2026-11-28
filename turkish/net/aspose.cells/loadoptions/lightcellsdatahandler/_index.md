---
title: "LoadOptions.LightCellsDataHandler"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LoadOptions özelliği. Şablon dosyası okunurken hücre verilerini işlemek için veri işleyicisi"
type: docs
url: /tr/net/aspose.cells/loadoptions/lightcellsdatahandler/
---
## LoadOptions.LightCellsDataHandler property

Şablon dosyası okunurken hücre verilerini işlemek için veri işleyicisi.

```csharp
public LightCellsDataHandler LightCellsDataHandler { get; set; }
```

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyLightCellsDataHandlerDemo
    {
        public static void Run()
        {
            // Hücre verilerini işlemek için özel bir LightCellsDataHandler oluştur
            var dataHandler = new CustomLightCellsDataHandler();
            
            // Yükleme seçeneklerini oluştur ve veri işleyicisini ayarla
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.LightCellsDataHandler = dataHandler;

            // Çalışma kitabını özel işleyiciyle yükle
            using (Workbook workbook = new Workbook("sample.xlsx", loadOptions))
            {
                Console.WriteLine("Workbook processed successfully with LightCellsDataHandler");
            }
        }
    }

    public class CustomLightCellsDataHandler : LightCellsDataHandler
    {
        public bool StartSheet(Worksheet sheet)
        {
            Console.WriteLine($"Processing sheet: {sheet.Name}");
            return true; // Continue processing this sheet
        }

        public bool StartRow(int rowIndex)
        {
            Console.WriteLine($"  Starting row: {rowIndex}");
            return true; // Continue processing this row
        }

        public bool ProcessRow(Row row)
        {
            // Gerekirse burada satır verilerini işleyebilirsiniz
            return true;
        }

        public bool StartCell(int columnIndex)
        {
            Console.WriteLine($"    Starting cell at column: {columnIndex}");
            return true; // Continue processing this cell
        }

        public bool ProcessCell(Cell cell)
        {
            Console.WriteLine($"      Cell[{cell.Row},{cell.Column}]: {cell.Value}");
            return true;
        }
    }
}
```

### Ayrıca Bakınız

* interface [LightCellsDataHandler](../../lightcellsdatahandler/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


