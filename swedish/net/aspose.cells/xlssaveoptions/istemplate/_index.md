---
title: "XlsSaveOptions.IsTemplate"
second_title: "Aspose.Cells för .NET API‑referens"
description: "XlsSaveOptions‑egenskap. Anger om en mallfil sparas"
type: docs
url: /sv/net/aspose.cells/xlssaveoptions/istemplate/
---
## XlsSaveOptions.IsTemplate property

Anger om en mallfil sparas.

```csharp
[Obsolete("Use XlsSaveOptions(SaveFormat.Xlt) when it is template, otherwise use XlsSaveOptions().")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsTemplate { get; set; }
```

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Skapa istället XlsSaveOptions med motsvarande sparformat (xlt för true och xls för false). Denna metod kommer att tas bort 12 månader senare från och med augusti 2020. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XlsSaveOptionsPropertyIsTemplateDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till exempeldata i det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Template");
            
            // Spara som mallfil
            string outputPath = "output_template.xlt";
            XlsSaveOptions saveOptions = new XlsSaveOptions();
            saveOptions.IsTemplate = true;
            
            using (FileStream fs = File.Create(outputPath))
            {
                workbook.Save(fs, saveOptions);
            }
            
            // Verifiera det sparade filformatet
            Workbook loadedWorkbook = new Workbook(outputPath);
            Console.WriteLine("File format: " + loadedWorkbook.FileFormat);
        }
    }
}
```

### Se även

* class [XlsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


