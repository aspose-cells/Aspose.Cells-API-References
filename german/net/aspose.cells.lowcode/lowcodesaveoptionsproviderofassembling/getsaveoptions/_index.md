---
title: "LowCodeSaveOptionsProviderOfAssembling.GetSaveOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LowCodeSaveOptionsProviderOfAssembling method. Gibt die Speicheroptionen zurück, aus denen die Ausgabeeinstellungen für den aktuell gesplitteten Teil abgerufen werden"
type: docs
url: /de/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/getsaveoptions/
---
## LowCodeSaveOptionsProviderOfAssembling.GetSaveOptions method

Liest die Speicheroptionen, aus denen die Ausgabeeinstellungen für das aktuelle geteilte Teil abgerufen werden.

```csharp
public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo part)
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfAssemblingMethodGetSaveOptionsWithSplitPartInfoDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Name = "DataSheet";
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].Value = "Sample Data for Split";

            try
            {
                // Erstelle eine Instanz von LowCodeSaveOptionsProviderOfAssembling
                var provider = new LowCodeSaveOptionsProviderOfAssembling
                {
                    PathHeader = "Output/",
                    PathTail = ".xlsx",
                    UseSheetName = true,
                    SheetPrefix = "Sheet_",
                    SplitPartPrefix = "Part_",
                    SaveOptionsTemplate = new LowCodeSaveOptions { SaveFormat = SaveFormat.Xlsx }
                };

                // Erstellen Sie eine SplitPartInfo‑Instanz mittels Reflexion, da der Konstruktor nicht zugänglich ist
                var splitPartInfo = (SplitPartInfo)Activator.CreateInstance(typeof(SplitPartInfo), nonPublic: true);

                // Rufen Sie GetSaveOptions mit dem SplitPartInfo‑Parameter auf
                LowCodeSaveOptions saveOptions = provider.GetSaveOptions(splitPartInfo);

                Console.WriteLine("SaveOptions created successfully");
                Console.WriteLine($"Output format: {saveOptions.SaveFormat}");

                // Speichern Sie die Arbeitsmappe (bei realer Verwendung würden die generierten Speicheroptionen verwendet)
                workbook.Save("GetSaveOptionsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in GetSaveOptions demo: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [SplitPartInfo](../../splitpartinfo/)
* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


