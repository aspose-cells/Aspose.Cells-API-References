---
title: "VbaProject.ValidatePassword"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método VbaProject. Valida la contraseña de protección"
type: docs
url: /es/net/aspose.cells.vba/vbaproject/validatepassword/
---
## VbaProject.ValidatePassword method

Valida la contraseña de protección.

```csharp
public bool ValidatePassword(string password)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| contraseña | String | la contraseña |

### Valor de retorno

Indica si la contraseña es la contraseña de protección de este proyecto VBA

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VbaProjectMethodValidatePasswordWithStringDemo
    {
        public static void Run()
        {
            // Crear objeto de libro de trabajo a partir de un archivo Excel de ejemplo con proyecto VBA
            Workbook workbook = new Workbook("example.xlsm");
            
            // Validar la contraseña del proyecto VBA
            bool isValid = workbook.VbaProject.ValidatePassword("test");
            
            // Mostrar el resultado de la validación
            Console.WriteLine("Password validation result: " + isValid);
        }
    }
}
```

### Ver también

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


