---
title: "Worksheet.Protect"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-metod. Skyddar kalkylbladet"
type: docs
url: /sv/net/aspose.cells/worksheet/protect/
---
## Protect(ProtectionType) {#protect}

Skyddar kalkylbladet.

```csharp
public void Protect(ProtectionType type)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| typ | ProtectionType | Skyddstyp. |

### Anmärkningar

Denna metod skyddar kalkylbladet utan lösenord. Den kan skydda kalkylbladet i alla versioner av Excel-filen.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodProtectWithProtectionTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet sheet = workbook.Worksheets[0];
            
            // Skydda kalkylbladet med skyddstypen Objects
            sheet.Protect(ProtectionType.Objects);
            
            // Spara arbetsboken
            workbook.Save("ProtectedWorksheet.xlsx");
        }
    }
}
```

### Se även

* enum [ProtectionType](../../protectiontype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Protect(ProtectionType, string, string) {#protect_1}

Skyddar kalkylbladet.

```csharp
public void Protect(ProtectionType type, string password, string oldPassword)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| typ | ProtectionType | Skyddstyp. |
| lösenord | String | Lösenord. |
| oldPassword | String | Om kalkylbladet redan är skyddat med ett lösenord, ange det gamla lösenordet. Annars kan du sätta ett null‑värde eller en tom sträng för denna parameter. |

### Anmärkningar

Denna metod kan skydda kalkylbladet i alla versioner av Excel-filen.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodProtectWithProtectionTypeStringStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skydda kalkylbladet med lösenord och tillåt alla skyddstyper
            worksheet.Protect(ProtectionType.All, "password123", null);
            
            // Spara arbetsboken
            workbook.Save("ProtectedWorksheet.xlsx");
        }
    }
}
```

### Se även

* enum [ProtectionType](../../protectiontype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


