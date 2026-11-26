---
title: "VbaProject.Protect"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método VbaProject. Protege o desprotege este proyecto VBA"
type: docs
url: /es/net/aspose.cells.vba/vbaproject/protect/
---
## VbaProject.Protect method

Protege o desprotege este proyecto VBA.

```csharp
public void Protect(bool islockedForViewing, string password)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| islockedForViewing | Booleano | indica si bloquea el proyecto para su visualización. |
| contraseña | String | Si el valor es nulo, desprotege este proyecto VBA; de lo contrario, protege este proyecto VBA. |

### Observaciones

Si islockedForViewing es verdadero, la contraseña no puede ser nula.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VbaProjectMethodProtectWithBooleanStringDemo
    {
        public static void Run()
        {
            // Crear un libro con proyecto VBA
            Workbook workbook = new Workbook();
            workbook.VbaProject.Protect(false, "password123");
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsm", SaveFormat.Xlsm);
        }
    }
}
```

### Ver también

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


