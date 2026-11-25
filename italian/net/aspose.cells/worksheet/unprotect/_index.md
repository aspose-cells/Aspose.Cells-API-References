---
title: "Worksheet.Unprotect"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Worksheet. Rimuove la protezione dal foglio di lavoro"
type: docs
url: /it/net/aspose.cells/worksheet/unprotect/
---
## Unprotect() {#unprotect}

Rimuove la protezione del worksheet.

```csharp
public void Unprotect()
```

### Osservazioni

Questo metodo rimuove la protezione dal foglio di lavoro che è protetto senza password.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetMethodUnprotectDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Proteggi il foglio di lavoro con una password
            worksheet.Protect(ProtectionType.All, "password123", null);
            Console.WriteLine("Worksheet is protected: " + worksheet.IsProtected);
            
            try
            {
                // Rimuovi la protezione dal foglio di lavoro senza password (dovrebbe fallire)
                worksheet.Unprotect();
                Console.WriteLine("Worksheet unprotected without password: " + !worksheet.IsProtected);
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error when trying to unprotect without password: " + ex.Message);
            }

            try
            {
                // Rimuovi la protezione dal foglio di lavoro con password errata (dovrebbe fallire)
                worksheet.Unprotect("wrongpassword");
                Console.WriteLine("Worksheet unprotected with wrong password: " + !worksheet.IsProtected);
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error when trying to unprotect with wrong password: " + ex.Message);
            }

            try
            {
                // Rimuovi la protezione del foglio di lavoro con la password corretta
                worksheet.Unprotect("password123");
                Console.WriteLine("Worksheet successfully unprotected: " + !worksheet.IsProtected);
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error when trying to unprotect: " + ex.Message);
            }
            
            // Salva il risultato
            workbook.Save("WorksheetMethodUnprotectDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Unprotect(string) {#unprotect_1}

Rimuove la protezione del worksheet.

```csharp
public void Unprotect(string password)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| password | String | Password |

### Osservazioni

Se il foglio di lavoro è protetto senza password, è possibile impostare un valore null o una stringa vuota al parametro password.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodUnprotectWithStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Proteggi il foglio di lavoro con password e tipo di protezione predefinito
            worksheet.Protect(ProtectionType.All, "test", null);
            
            // Rimuovi la protezione del foglio di lavoro con password
            worksheet.Unprotect("test");
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


