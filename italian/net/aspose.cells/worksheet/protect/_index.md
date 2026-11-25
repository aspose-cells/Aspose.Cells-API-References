---
title: "Worksheet.Protect"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Worksheet. Protegge il foglio di lavoro"
type: docs
url: /it/net/aspose.cells/worksheet/protect/
---
## Protect(ProtectionType) {#protect}

Protegge il worksheet.

```csharp
public void Protect(ProtectionType type)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | ProtectionType | Tipo di protezione. |

### Osservazioni

Questo metodo protegge il foglio di lavoro senza password. Può proteggere il foglio di lavoro in tutte le versioni del file Excel.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodProtectWithProtectionTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet sheet = workbook.Worksheets[0];
            
            // Proteggi il foglio di lavoro con il tipo di protezione Objects
            sheet.Protect(ProtectionType.Objects);
            
            // Salva la cartella di lavoro
            workbook.Save("ProtectedWorksheet.xlsx");
        }
    }
}
```

### Vedi anche

* enum [ProtectionType](../../protectiontype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Protect(ProtectionType, string, string) {#protect_1}

Protegge il worksheet.

```csharp
public void Protect(ProtectionType type, string password, string oldPassword)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | ProtectionType | Tipo di protezione. |
| password | String | Password. |
| oldPassword | String | Se il foglio di lavoro è già protetto da una password, fornisci la vecchia password. Altrimenti, puoi impostare un valore null o una stringa vuota per questo parametro. |

### Osservazioni

Questo metodo può proteggere il foglio di lavoro in tutte le versioni del file Excel.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodProtectWithProtectionTypeStringStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Proteggi il foglio di lavoro con password e consenti tutti i tipi di protezione
            worksheet.Protect(ProtectionType.All, "password123", null);
            
            // Salva la cartella di lavoro
            workbook.Save("ProtectedWorksheet.xlsx");
        }
    }
}
```

### Vedi anche

* enum [ProtectionType](../../protectiontype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


