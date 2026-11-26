---
title: "Clase WriteProtection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.WriteProtection. Especifica la configuración de protección contra escritura para un libro de trabajo"
type: docs
url: /es/net/aspose.cells/writeprotection/
---
## WriteProtection class

Especifica la configuración de protección contra escritura para un libro de trabajo.

```csharp
public class WriteProtection
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Author](../../aspose.cells/writeprotection/author/) { get; set; } | Obtiene y establece el autor. |
| [IsWriteProtected](../../aspose.cells/writeprotection/iswriteprotected/) { get; } | Indica si este libro de trabajo está protegido contra escritura. |
| [Password](../../aspose.cells/writeprotection/password/) { get; set; } | Establece la contraseña de protección para modificar el archivo. |
| [RecommendReadOnly](../../aspose.cells/writeprotection/recommendreadonly/) { get; set; } | Indica si la opción Leer solo recomendado está seleccionada. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [ValidatePassword](../../aspose.cells/writeprotection/validatepassword/)(string) | Devuelve true si la contraseña especificada es la misma que la contraseña de protección contra escritura con la que se protegió el archivo. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WriteProtectionDemo
    {
        public static void WriteProtectionExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la configuración del libro de trabajo
            WorkbookSettings settings = workbook.Settings;

            // Acceder a la configuración de protección contra escritura
            WriteProtection writeProtection = settings.WriteProtection;

            // Establecer el autor de la protección contra escritura
            writeProtection.Author = "John Doe";

            // Establecer la contraseña para la protección contra escritura
            writeProtection.Password = "password123";

            // Establecer la opción recomendada de solo lectura
            writeProtection.RecommendReadOnly = true;

            // Verificar si el libro de trabajo está protegido contra escritura
            bool isWriteProtected = writeProtection.IsWriteProtected;
            Console.WriteLine("Is Write Protected: " + isWriteProtected);

            // Validar la contraseña
            bool isValidPassword = writeProtection.ValidatePassword("password123");
            Console.WriteLine("Is Valid Password: " + isValidPassword);

            // Guarda el libro de trabajo
            workbook.Save("WriteProtectionExample.xlsx");

            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


