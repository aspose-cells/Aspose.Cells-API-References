---
title: "SaveOptions.EncryptDocumentProperties"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SaveOptions-egenskap. Anger om dokumentegenskaper ska krypteras när du sparar som .xls-fil. Standardvärdet är true"
type: docs
url: /sv/net/aspose.cells/saveoptions/encryptdocumentproperties/
---
## SaveOptions.EncryptDocumentProperties property

Indikerar om dokumentegenskaper ska krypteras när du sparar som .xls-fil. Standardvärdet är true.

```csharp
public bool EncryptDocumentProperties { get; set; }
```

### Anmärkningar

Endast för .xls, .xlsx, .xlsb och .xlsm-filer.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyEncryptDocumentPropertiesDemo
    {
        public static void Run()
        {
            // Skapa en exempelarbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ställ in några dokumentegenskaper
            workbook.BuiltInDocumentProperties.Author = "Test Author";
            workbook.BuiltInDocumentProperties.Title = "Test Document";
            
            // Ställ in lösenordsskydd
            workbook.Settings.Password = "password123";
            
            // Spara med EncryptDocumentProperties = true (standard)
            XlsSaveOptions saveOptions1 = new XlsSaveOptions();
            saveOptions1.EncryptDocumentProperties = true;
            workbook.Save("encrypted_properties.xls", saveOptions1);
            
            // Spara med EncryptDocumentProperties = false
            XlsSaveOptions saveOptions2 = new XlsSaveOptions();
            saveOptions2.EncryptDocumentProperties = false;
            workbook.Save("unencrypted_properties.xls", saveOptions2);
            
            // Verifiera genom att ladda tillbaka
            Console.WriteLine("Files saved. Try opening them to see the difference in property encryption.");
        }
    }
}
```

### Se även

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


