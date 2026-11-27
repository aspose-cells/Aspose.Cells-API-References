---
title: "Worksheet.Unprotect"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-metod. Låser upp arbetsbladet"
type: docs
url: /sv/net/aspose.cells/worksheet/unprotect/
---
## Unprotect() {#unprotect}

Avskyddar kalkylbladet.

```csharp
public void Unprotect()
```

### Anmärkningar

Denna metod låser upp arbetsbladet som är skyddat utan lösenord.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetMethodUnprotectDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skydda arbetsbladet med ett lösenord
            worksheet.Protect(ProtectionType.All, "password123", null);
            Console.WriteLine("Worksheet is protected: " + worksheet.IsProtected);
            
            try
            {
                // Lås upp arbetsbladet utan lösenord (bör misslyckas)
                worksheet.Unprotect();
                Console.WriteLine("Worksheet unprotected without password: " + !worksheet.IsProtected);
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error when trying to unprotect without password: " + ex.Message);
            }

            try
            {
                // Lås upp arbetsbladet med fel lösenord (bör misslyckas)
                worksheet.Unprotect("wrongpassword");
                Console.WriteLine("Worksheet unprotected with wrong password: " + !worksheet.IsProtected);
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error when trying to unprotect with wrong password: " + ex.Message);
            }

            try
            {
                // Lås upp arbetsbladet med korrekt lösenord
                worksheet.Unprotect("password123");
                Console.WriteLine("Worksheet successfully unprotected: " + !worksheet.IsProtected);
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error when trying to unprotect: " + ex.Message);
            }
            
            // Spara resultatet
            workbook.Save("WorksheetMethodUnprotectDemo.xlsx");
        }
    }
}
```

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Unprotect(string) {#unprotect_1}

Avskyddar kalkylbladet.

```csharp
public void Unprotect(string password)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| lösenord | String | Lösenord |

### Anmärkningar

Om arbetsbladet är skyddat utan lösenord kan du sätta ett null‑värde eller en tom sträng till lösenordsparametern.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodUnprotectWithStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skydda arbetsbladet med lösenord och standardskyddstyp
            worksheet.Protect(ProtectionType.All, "test", null);
            
            // Lås upp arbetsbladet med lösenord
            worksheet.Unprotect("test");
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


