---
title: "SaveOptions.EncryptDocumentProperties"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SaveOptions-Eigenschaft. Gibt an, ob Dokumenteneigenschaften beim Speichern als .xls-Datei verschlüsselt werden. Der Standardwert ist true"
type: docs
url: /de/net/aspose.cells/saveoptions/encryptdocumentproperties/
---
## SaveOptions.EncryptDocumentProperties property

Gibt an, ob Dokumenteigenschaften beim Speichern als .xls-Datei verschlüsselt werden. Der Standardwert ist true.

```csharp
public bool EncryptDocumentProperties { get; set; }
```

### Hinweise

Nur für .xls, .xlsx, .xlsb und .xlsm Dateien.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyEncryptDocumentPropertiesDemo
    {
        public static void Run()
        {
            // Erstelle ein Beispielarbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Einige Dokumenteigenschaften festlegen
            workbook.BuiltInDocumentProperties.Author = "Test Author";
            workbook.BuiltInDocumentProperties.Title = "Test Document";
            
            // Passwortschutz festlegen
            workbook.Settings.Password = "password123";
            
            // Speichern mit EncryptDocumentProperties = true (Standard)
            XlsSaveOptions saveOptions1 = new XlsSaveOptions();
            saveOptions1.EncryptDocumentProperties = true;
            workbook.Save("encrypted_properties.xls", saveOptions1);
            
            // Speichern mit EncryptDocumentProperties = false
            XlsSaveOptions saveOptions2 = new XlsSaveOptions();
            saveOptions2.EncryptDocumentProperties = false;
            workbook.Save("unencrypted_properties.xls", saveOptions2);
            
            // Durch erneutes Laden verifizieren
            Console.WriteLine("Files saved. Try opening them to see the difference in property encryption.");
        }
    }
}
```

### Siehe auch

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


