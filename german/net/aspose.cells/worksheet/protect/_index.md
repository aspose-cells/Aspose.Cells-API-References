---
title: "Worksheet.Protect"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Methode. Schützt das Arbeitsblatt"
type: docs
url: /de/net/aspose.cells/worksheet/protect/
---
## Protect(ProtectionType) {#protect}

Schützt das Arbeitsblatt.

```csharp
public void Protect(ProtectionType type)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Typ | ProtectionType | Schutztyp. |

### Hinweise

Diese Methode schützt das Arbeitsblatt ohne Passwort. Sie kann das Arbeitsblatt in allen Excel-Versionen schützen.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodProtectWithProtectionTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet sheet = workbook.Worksheets[0];
            
            // Schützt das Arbeitsblatt mit dem Schutztyp Objects
            sheet.Protect(ProtectionType.Objects);
            
            // Speichere die Arbeitsmappe
            workbook.Save("ProtectedWorksheet.xlsx");
        }
    }
}
```

### Siehe auch

* enum [ProtectionType](../../protectiontype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Protect(ProtectionType, string, string) {#protect_1}

Schützt das Arbeitsblatt.

```csharp
public void Protect(ProtectionType type, string password, string oldPassword)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Typ | ProtectionType | Schutztyp. |
| Passwort | String | Passwort. |
| oldPassword | String | Wenn das Arbeitsblatt bereits durch ein Passwort geschützt ist, geben Sie bitte das alte Passwort an. Andernfalls können Sie für diesen Parameter einen Nullwert oder eine leere Zeichenfolge festlegen. |

### Hinweise

Diese Methode kann das Arbeitsblatt in allen Excel-Versionen schützen.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodProtectWithProtectionTypeStringStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Schützt das Arbeitsblatt mit Passwort und erlaubt alle Schutztypen
            worksheet.Protect(ProtectionType.All, "password123", null);
            
            // Speichere die Arbeitsmappe
            workbook.Save("ProtectedWorksheet.xlsx");
        }
    }
}
```

### Siehe auch

* enum [ProtectionType](../../protectiontype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


