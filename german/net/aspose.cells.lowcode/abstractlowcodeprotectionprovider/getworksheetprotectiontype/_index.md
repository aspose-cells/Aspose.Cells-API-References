---
title: "AbstractLowCodeProtectionProvider.GetWorksheetProtectionType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AbstractLowCodeProtectionProvider-Methode. Gibt den Schutztyp zurück, um das angegebene Arbeitsblatt zu schützen"
type: docs
url: /de/net/aspose.cells.lowcode/abstractlowcodeprotectionprovider/getworksheetprotectiontype/
---
## AbstractLowCodeProtectionProvider.GetWorksheetProtectionType method

Liefert den Schutztyp zum Schützen des angegebenen Arbeitsblatts.

```csharp
public virtual ProtectionType GetWorksheetProtectionType(string sheetName)
```

### Rückgabewert

Schutztyp zum Schutz des angegebenen Arbeitsblatts. None bedeutet, dass das Arbeitsblatt nicht geschützt ist.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class AbstractLowCodeProtectionProviderMethodGetWorksheetProtectionTypeWithStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets.Add("newSheet");
            string name = worksheet.Name;
            var protectionProvider = new CustomProtectionProvider();

            try
            {
                worksheet.Protect(protectionProvider.GetWorksheetProtectionType(name), protectionProvider.GetWorksheetPassword(name), "");
               
                // Ergebnis anzeigen
                Console.WriteLine($"Worksheet '{name}' protection type: {protectionProvider.GetWorksheetProtectionType(name)}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error retrieving protection type: {ex.Message}");
            }

            // Speichere die Arbeitsmappe
            workbook.Save("GetWorksheetProtectionTypeDemo.xlsx");
        }

        private class CustomProtectionProvider : AbstractLowCodeProtectionProvider
        {
            public override ProtectionType GetWorksheetProtectionType(string sheetName)
            {
                return ProtectionType.Structure;
            }

            public override string GetWorksheetPassword(string sheetName)
            {
                return $"aspose123_{sheetName}";
            }
        }

    }
    
}
```

### Siehe auch

* enum [ProtectionType](../../../aspose.cells/protectiontype/)
* class [AbstractLowCodeProtectionProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


