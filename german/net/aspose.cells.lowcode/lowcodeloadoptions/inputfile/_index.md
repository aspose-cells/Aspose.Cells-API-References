---
title: "LowCodeLoadOptions.InputFile"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LowCodeLoadOptions-Eigenschaft. Liest und setzt den Dateipfad der Vorlage, falls erforderlich"
type: docs
url: /de/net/aspose.cells.lowcode/lowcodeloadoptions/inputfile/
---
## LowCodeLoadOptions.InputFile property

Liest und setzt die Datei (mit Pfad, falls nötig) der Vorlage.

```csharp
public string InputFile { get; set; }
```

### Hinweise

Wenn für diese Eigenschaft ein nicht‑null und nicht‑leerer Pfad festgelegt wird, wird der zuvor gesetzte Wert für [`InputStream`](../inputstream/) ignoriert.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeLoadOptionsPropertyInputFileDemo
    {
        public static void Run()
        {
            // Erstelle und speichere eine Beispielvorlagendatei
            Workbook templateWorkbook = new Workbook();
            templateWorkbook.Worksheets[0].Cells["A1"].PutValue("Template Value");
            const string templatePath = "LowCodeTemplate.xlsx";
            templateWorkbook.Save(templatePath);

            // Initialisiere LowCodeLoadOptions und demonstriere die InputFile‑Eigenschaft
            LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
            Console.WriteLine("Initial InputFile value: " + loadOptions.InputFile);

            // Setze die InputFile‑Eigenschaft, um unsere Vorlage zu verwenden
            loadOptions.InputFile = templatePath;
            Console.WriteLine("Updated InputFile value: " + loadOptions.InputFile);

            // Lade die Arbeitsmappe mit der angegebenen Vorlagendatei
            Workbook workbook = new Workbook(loadOptions.InputFile);
            
            // Modifiziere die geladene Vorlage
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A2"].PutValue("Added using InputFile: " + loadOptions.InputFile);

            // Speichere die geänderte Arbeitsmappe
            workbook.Save("PropertyInputFileDemo_Output.xlsx");
        }
    }
}
```

### Siehe auch

* class [LowCodeLoadOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


