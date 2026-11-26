---
title: "WorkbookSettings.IsEncrypted"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookSettings. Obtiene un valor que indica si se requiere una contraseña para abrir este libro de trabajo"
type: docs
url: /es/net/aspose.cells/workbooksettings/isencrypted/
---
## WorkbookSettings.IsEncrypted property

Obtiene un valor que indica si se requiere una contraseña para abrir este libro.

```csharp
public bool IsEncrypted { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyIsEncryptedDemo
    {
        public static void Run()
        {
            // Ejemplo 1: Verificar si un libro de trabajo protegido con contraseña está encriptado
            string encryptedFilePath = "encrypted.xlsx";
            var encryptedWorkbook = new Workbook(encryptedFilePath, new LoadOptions { Password = "password" });
            Console.WriteLine($"Encrypted workbook IsEncrypted: {encryptedWorkbook.Settings.IsEncrypted}");

            // Ejemplo 2: Verificar si un libro de trabajo normal está encriptado
            string normalFilePath = "normal.xlsx";
            var normalWorkbook = new Workbook(normalFilePath);
            Console.WriteLine($"Normal workbook IsEncrypted: {normalWorkbook.Settings.IsEncrypted}");

            // Ejemplo 3: Crear y guardar un libro de trabajo encriptado
            var newWorkbook = new Workbook();
            newWorkbook.Settings.Password = "12345";
            newWorkbook.Save("new_encrypted.xlsx");
            Console.WriteLine($"New workbook IsEncrypted: {newWorkbook.Settings.IsEncrypted}");
        }
    }
}
```

### Ver también

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


