---
title: "Classe WriteProtection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.WriteProtection. Specifica le impostazioni di protezione in scrittura per una cartella di lavoro"
type: docs
url: /it/net/aspose.cells/writeprotection/
---
## WriteProtection class

Specifica le impostazioni di protezione in scrittura per una cartella di lavoro.

```csharp
public class WriteProtection
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Author](../../aspose.cells/writeprotection/author/) { get; set; } | Ottiene e imposta l'autore. |
| [IsWriteProtected](../../aspose.cells/writeprotection/iswriteprotected/) { get; } | Indica se questa cartella di lavoro è protetta in scrittura. |
| [Password](../../aspose.cells/writeprotection/password/) { get; set; } | Imposta la password di protezione per modificare il file. |
| [RecommendReadOnly](../../aspose.cells/writeprotection/recommendreadonly/) { get; set; } | Indica se l'opzione Consiglia sola lettura è selezionata. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [ValidatePassword](../../aspose.cells/writeprotection/validatepassword/)(string) | Restituisce true se la password specificata è la stessa della password di protezione in scrittura con cui il file è stato protetto. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WriteProtectionDemo
    {
        public static void WriteProtectionExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi alle impostazioni della cartella di lavoro
            WorkbookSettings settings = workbook.Settings;

            // Accedi alle impostazioni di protezione in scrittura
            WriteProtection writeProtection = settings.WriteProtection;

            // Imposta l'autore della protezione in scrittura
            writeProtection.Author = "John Doe";

            // Imposta la password per la protezione in scrittura
            writeProtection.Password = "password123";

            // Imposta l'opzione di sola lettura consigliata
            writeProtection.RecommendReadOnly = true;

            // Verifica se la cartella di lavoro è protetta in scrittura
            bool isWriteProtected = writeProtection.IsWriteProtected;
            Console.WriteLine("Is Write Protected: " + isWriteProtected);

            // Convalida la password
            bool isValidPassword = writeProtection.ValidatePassword("password123");
            Console.WriteLine("Is Valid Password: " + isValidPassword);

            // Salva la cartella di lavoro
            workbook.Save("WriteProtectionExample.xlsx");

            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


