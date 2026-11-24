---
title: "LowCodeSaveOptionsProviderOfAssembling.UseSheetName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LowCodeSaveOptionsProviderOfAssembling property. Gibt an, ob der Dateipfad mit dem Blattnamen anstelle des Blattindexes erstellt wird. Standardwert ist false"
type: docs
url: /de/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/usesheetname/
---
## LowCodeSaveOptionsProviderOfAssembling.UseSheetName property

Ob der Dateipfad mit dem Blattnamen anstelle des Blatt‑Index erstellt wird. Standardwert ist false.

```csharp
public bool UseSheetName { get; set; }
```

### Hinweise

Der Blattname wird niemals automatisch neu erstellt. Wenn er also auf true gesetzt wird, stellen Sie bitte sicher, dass kein spezieller Blattname vorhanden ist, der einen ungültigen Dateipfad oder -namen verursachen könnte.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfAssemblingPropertyUseSheetNameDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine neue Arbeitsmappe mit benanntem Arbeitsblatt
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Name = "MonthlyReport";
            
            // Fügen Sie Beispieldaten für die Split‑Demonstration hinzu
            for(int i = 0; i < 15; i++)
            {
                worksheet.Cells[$"A{i+1}"].PutValue($"Record {i+1}");
            }

            // Erstellen und konfigurieren Sie den Provider
            var provider = new LowCodeSaveOptionsProviderOfAssembling
            {
                PathHeader = "split_files/",
                PathTail = ".xlsx",
                SheetPrefix = "Sheet_",
                SplitPartPrefix = "Part_",
                SaveOptionsTemplate = new LowCodeSaveOptions { SaveFormat = SaveFormat.Xlsx }
            };

            // Demonstrieren Sie UseSheetName=false (Standard)
            Console.WriteLine($"Default UseSheetName: {provider.UseSheetName}");
            workbook.Save("output_default", provider.SaveOptionsTemplate.SaveFormat);

            // Ändern Sie die Eigenschaft und demonstrieren Sie das neue Verhalten
            provider.UseSheetName = true;
            Console.WriteLine($"\nModified UseSheetName: {provider.UseSheetName}");
            workbook.Save("output_modified", provider.SaveOptionsTemplate.SaveFormat);

            Console.WriteLine("Check 'split_files' directory for output files with different naming schemes");
        }
    }
}
```

### Siehe auch

* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


