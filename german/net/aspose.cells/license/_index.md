---
title: "Klasse License"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Klasse Aspose.Cells.License. Stellt Methoden bereit, um die Komponente zu lizenzieren"
type: docs
url: /de/net/aspose.cells/license/
---
## License class

Stellt Methoden bereit, um die Komponente zu lizenzieren.

```csharp
public class License
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [License](license/)() | Initialisiert eine neue Instanz dieser Klasse. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [SetLicense](../../aspose.cells/license/setlicense/#setlicense)(Stream) | Lizenziert die Komponente. |
| [SetLicense](../../aspose.cells/license/setlicense/#setlicense_1)(string) | Lizenziert die Komponente. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class LicenseDemo
    {
        public static void LicenseExample()
        {
            // Erstellen Sie eine Instanz der License-Klasse
            License license = new License();

            // Setzen Sie die Lizenz mithilfe eines Lizenzdateinamens
            license.SetLicense("Aspose.Cells.NET.lic");

            // Alternativ setzen Sie die Lizenz mithilfe eines Streams
            using (FileStream licenseStream = new FileStream("Aspose.Cells.NET.lic", FileMode.Open))
            {
                license.SetLicense(licenseStream);
            }

            // Zusätzlicher Code, um die Verwendung der lizenzierten Aspose.Cells-Funktionalität zu demonstrieren
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells[0, 0].PutValue("Hello, Aspose.Cells!");

            // Speichern Sie die Arbeitsmappe, um zu überprüfen, ob die Lizenz korrekt angewendet wurde
            workbook.Save("LicensedWorkbook.xlsx");

            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


