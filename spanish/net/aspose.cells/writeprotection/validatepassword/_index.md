---
title: "WriteProtection.ValidatePassword"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método WriteProtection. Devuelve true si la contraseña especificada es la misma que la contraseña de protección contra escritura con la que el archivo fue protegido"
type: docs
url: /es/net/aspose.cells/writeprotection/validatepassword/
---
## WriteProtection.ValidatePassword method

Devuelve true si la contraseña especificada es la misma que la contraseña de protección contra escritura con la que se protegió el archivo.

```csharp
public bool ValidatePassword(string password)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| contraseña | String | La contraseña especificada. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WriteProtectionMethodValidatePasswordWithStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Establecer la contraseña de protección contra escritura
            workbook.Settings.WriteProtection.Password = "1234";
            
            // Validar contraseña
            Console.WriteLine("Password '1234' is valid: " + 
                workbook.Settings.WriteProtection.ValidatePassword("1234"));
            Console.WriteLine("Password 'wrong' is valid: " + 
                workbook.Settings.WriteProtection.ValidatePassword("wrong"));
        }
    }
}
```

### Ver también

* class [WriteProtection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


