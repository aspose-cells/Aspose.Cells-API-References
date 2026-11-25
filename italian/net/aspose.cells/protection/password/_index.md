---
title: "Protection.Password"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Protection. Rappresenta la password per proteggere il foglio di lavoro"
type: docs
url: /it/net/aspose.cells/protection/password/
---
## Protection.Password property

Rappresenta la password per proteggere il foglio di lavoro.

```csharp
public string Password { get; set; }
```

### Osservazioni

Se la password è impostata a null o a stringa vuota, è possibile sbloccare il foglio di lavoro o la cartella di lavoro senza utilizzare una password. In caso contrario, è necessario specificare la password per sbloccare il foglio di lavoro o la cartella di lavoro.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyPasswordDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Imposta le impostazioni di protezione con password
            Protection protection = worksheet.Protection;
            protection.AllowEditingContent = false;
            protection.AllowDeletingColumn = false;
            protection.Password = "test123";

            // Verifica la protezione con password
            Console.WriteLine("Worksheet is protected: " + (protection.Password != null));
            Console.WriteLine("Protection password: " + protection.Password);

            // Crea un altro oggetto Protection da confrontare
            Protection protection2 = worksheet.Protection;
            protection2.Password = "test123";

            // Confronta la protezione con password
            Console.WriteLine("Passwords match: " + (protection.Password == protection2.Password));
        }
    }
}
```

### Vedi anche

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


