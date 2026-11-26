---
title: "Enumeración EncryptionType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.EncryptionType. Tipo de cifrado. Solo se usa en excel2003. Encriptaremos el libro de trabajo 2007/2010 usando SHA AES de la misma forma que lo hace Excel y este EncryptionType será ignorado"
type: docs
url: /es/net/aspose.cells/encryptiontype/
---
## EncryptionType enumeration

Tipo de cifrado. Solo usado por excel2003. Encriptaremos libros de trabajo 2007/2010 usando SHA AES de la misma forma que lo hace Excel, y este EncryptionType será ignorado.

```csharp
public enum EncryptionType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| XOR | `0` | Algoritmo de cifrado XOR. |
| Compatible | `1` | Compatible con Office 97/2000. |
| EnhancedCryptographicProviderV1 | `2` | Cifrado mejorado. |
| StrongCryptographicProvider | `3` | Algoritmo de cifrado fuerte. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class EncryptionTypeDemo
    {
        public static void EncryptionTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Establecer opciones de cifrado para el libro de trabajo
            EncryptionType encryptionType = EncryptionType.EnhancedCryptographicProviderV1;
            int keyLength = 128; // Key length can be 40, 128, or 256 bits

            // Aplicar configuraciones de cifrado
            workbook.SetEncryptionOptions(encryptionType, keyLength);

            // Proteger el libro de trabajo con una contraseña
            string password = "securePassword";
            workbook.Protect(ProtectionType.All, password);

            // Guarda el libro de trabajo
            workbook.Save("EncryptedWorkbook.xlsx");
            workbook.Save("EncryptedWorkbook.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


