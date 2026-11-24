---
title: "OoxmlSaveOptions.ExportCellName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "OoxmlSaveOptions-Eigenschaft. Gibt an, ob Zellnamen in Excel2007-Dateien (.xlsx, .xlsm, .xltx, .xltm) exportiert werden. Wenn die Ausgabedatei von SQL Server DTS verwendet werden kann, muss dieser Wert true sein. Das Setzen des Werts auf false erhöht die Leistung erheblich und reduziert die Dateigröße beim Erstellen großer Dateien. Der Standardwert ist true."
type: docs
url: /de/net/aspose.cells/ooxmlsaveoptions/exportcellname/
---
## OoxmlSaveOptions.ExportCellName property

Gibt an, ob Zellnamen in eine Excel2007 .xlsx (.xlsm, .xltx, .xltm)-Datei exportiert werden. Wenn auf die Ausgabedatei von SQL Server DTS zugegriffen werden kann, muss dieser Wert true sein. Das Setzen des Werts auf false erhöht die Leistung erheblich und reduziert die Dateigröße beim Erstellen großer Dateien. Der Standardwert ist true.

```csharp
public bool ExportCellName { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OoxmlSaveOptionsPropertyExportCellNameDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie einige Daten in Zellen ein
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B2"].PutValue(123);
            
            // Erstellen Sie XLSX-Speicheroptionen mit aktiviertem ExportCellName
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.ExportCellName = true;
            
            // Speichern Sie die Arbeitsmappe mit exportierten Zellnamen
            workbook.Save("output_with_cellnames.xlsx", saveOptions);
            
            // Erstellen Sie weitere Speicheroptionen mit deaktiviertem ExportCellName (Standard)
            OoxmlSaveOptions saveOptions2 = new OoxmlSaveOptions();
            
            // Speichern Sie die Arbeitsmappe ohne exportierte Zellnamen
            workbook.Save("output_without_cellnames.xlsx", saveOptions2);
        }
    }
}
```

### Siehe auch

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


