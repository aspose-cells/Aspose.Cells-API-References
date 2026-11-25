---
title: "FileFormatUtil.VerifyPassword"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo FileFormatUtil. Rileva e restituisce le informazioni sul formato di un Excel memorizzato in uno stream"
type: docs
url: /it/net/aspose.cells/fileformatutil/verifypassword/
---
## FileFormatUtil.VerifyPassword method

Rileva e restituisce le informazioni sul formato di un file Excel memorizzato in uno stream.

```csharp
public static bool VerifyPassword(Stream stream, string password)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | Stream |  |
| password | String | La password per i file ooxml crittografati. |

### Valore di ritorno

Restituisce se la password è corretta.

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatUtilMethodVerifyPasswordWithStreamStringDemo
    {
        public static void Run()
        {
            string filePath = "example.xlsx";
            string correctPassword = "test";
            string wrongPassword = "1234";

            using (Stream stream = File.OpenRead(filePath))
            {
                bool isValid = FileFormatUtil.VerifyPassword(stream, correctPassword);
                Console.WriteLine($"Password '{correctPassword}' is valid: {isValid}");
            }

            using (Stream stream = File.OpenRead(filePath))
            {
                bool isValid = FileFormatUtil.VerifyPassword(stream, wrongPassword);
                Console.WriteLine($"Password '{wrongPassword}' is valid: {isValid}");
            }
        }
    }
}
```

### Vedi anche

* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


