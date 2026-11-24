---
title: "Worksheet.Unprotect"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Methode. Hebt den Schutz des Arbeitsblatts auf"
type: docs
url: /de/net/aspose.cells/worksheet/unprotect/
---
## Unprotect() {#unprotect}

Hebt den Schutz des Arbeitsblatts auf.

```csharp
public void Unprotect()
```

### Hinweise

Diese Methode hebt den Schutz eines Arbeitsblatts auf, das ohne Passwort geschützt ist.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetMethodUnprotectDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Schütze das Arbeitsblatt mit einem Passwort
            worksheet.Protect(ProtectionType.All, "password123", null);
            Console.WriteLine("Worksheet is protected: " + worksheet.IsProtected);
            
            try
            {
                // Entferne den Schutz des Arbeitsblatts ohne Passwort (sollte fehlschlagen)
                worksheet.Unprotect();
                Console.WriteLine("Worksheet unprotected without password: " + !worksheet.IsProtected);
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error when trying to unprotect without password: " + ex.Message);
            }

            try
            {
                // Entferne den Schutz des Arbeitsblatts mit falschem Passwort (sollte fehlschlagen)
                worksheet.Unprotect("wrongpassword");
                Console.WriteLine("Worksheet unprotected with wrong password: " + !worksheet.IsProtected);
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error when trying to unprotect with wrong password: " + ex.Message);
            }

            try
            {
                // Entferne den Schutz des Arbeitsblatts mit dem richtigen Passwort
                worksheet.Unprotect("password123");
                Console.WriteLine("Worksheet successfully unprotected: " + !worksheet.IsProtected);
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error when trying to unprotect: " + ex.Message);
            }
            
            // Ergebnis speichern
            workbook.Save("WorksheetMethodUnprotectDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Unprotect(string) {#unprotect_1}

Hebt den Schutz des Arbeitsblatts auf.

```csharp
public void Unprotect(string password)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Passwort | String | Passwort |

### Hinweise

Wenn das Arbeitsblatt ohne Passwort geschützt ist, können Sie dem Passwortparameter einen Nullwert oder eine leere Zeichenkette zuweisen.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodUnprotectWithStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Schütze das Arbeitsblatt mit Passwort und dem Standard-Schutztyp
            worksheet.Protect(ProtectionType.All, "test", null);
            
            // Entferne den Schutz des Arbeitsblatts mit Passwort
            worksheet.Unprotect("test");
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


