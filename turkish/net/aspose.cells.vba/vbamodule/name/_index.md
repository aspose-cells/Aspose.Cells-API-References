---
title: "VbaModule.Name"
second_title: "Aspose.Cells için .NET API Referansı"
description: "VbaModule özelliği. Modülün adını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.vba/vbamodule/name/
---
## VbaModule.Name property

Modülün adını alır ve ayarlar.

```csharp
public string Name { get; set; }
```

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaModulePropertyNameDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook wb = new Workbook();

            // Bir çalışma sayfası ekleyin ve onun VBA modülünü alın
            Worksheet sheet = wb.Worksheets[0];
            int moduleIndex = wb.VbaProject.Modules.Add(sheet);
            VbaModule module = wb.VbaProject.Modules[moduleIndex];

            // Modül adını ayarlayın
            module.Name = "Sheet1";

            // Modüle basit VBA kodu ekleyin
            string vbaCode = "Private Sub Worksheet_SelectionChange(ByVal Target As Range)\r\n" +
                             "    MsgBox \"Sheet name: \" & Me.Name\r\n" +
                             "End Sub\r\n";
            module.Codes = vbaCode;

            // Bellek akışına kaydedin (gösterim amaçlı)
            using (MemoryStream ms = new MemoryStream())
            {
                wb.Save(ms, SaveFormat.Xlsm);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [VbaModule](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


