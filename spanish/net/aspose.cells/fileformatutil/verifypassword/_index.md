---
title: "FileFormatUtil.VerifyPassword"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método FileFormatUtil. Detecta y devuelve la información sobre el formato de un Excel almacenado en un stream"
type: docs
url: /es/net/aspose.cells/fileformatutil/verifypassword/
---
## FileFormatUtil.VerifyPassword method

Detecta y devuelve la información sobre un formato de un Excel almacenado en un flujo.

```csharp
public static bool VerifyPassword(Stream stream, string password)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | Stream |  |
| contraseña | String | La contraseña para archivos ooxml encriptados. |

### Valor de retorno

Devuelve si la contraseña es correcta.

### Ejemplos

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

### Ver también

* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


