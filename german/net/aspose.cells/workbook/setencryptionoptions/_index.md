---
title: "Workbook.SetEncryptionOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook-Methode. Setze Verschlüsselungsoptionen"
type: docs
url: /de/net/aspose.cells/workbook/setencryptionoptions/
---
## Workbook.SetEncryptionOptions method

Verschlüsselungsoptionen festlegen.

```csharp
public void SetEncryptionOptions(EncryptionType encryptionType, int keyLength)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| encryptionType | EncryptionType | Der Verschlüsselungstyp. |
| keyLength | Int32 | Die Schlüssellänge. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodSetEncryptionOptionsWithEncryptionTypeInt32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Füge dem Arbeitsblatt einige Daten hinzu
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Encryption");
            
            // Passwort und Verschlüsselungsoptionen festlegen
            workbook.Settings.Password = "1234";
            workbook.SetEncryptionOptions(EncryptionType.StrongCryptographicProvider, 128);
            
            // Das verschlüsselte Arbeitsbuch speichern
            workbook.Save("EncryptedWorkbook.xls", SaveFormat.Excel97To2003);
            
            // Durch Laden des verschlüsselten Arbeitsbuchs verifizieren
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.Password = "1234";
            Workbook encryptedWorkbook = new Workbook("EncryptedWorkbook.xls", loadOptions);
            
            Console.WriteLine("Workbook encrypted and loaded successfully.");
        }
    }
}
```

### Siehe auch

* enum [EncryptionType](../../encryptiontype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


