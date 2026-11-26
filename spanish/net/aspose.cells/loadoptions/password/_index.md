---
title: "LoadOptions.Password"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LoadOptions. Obtiene y establece la contraseña del libro de trabajo"
type: docs
url: /es/net/aspose.cells/loadoptions/password/
---
## LoadOptions.Password property

Obtiene y establece la contraseña del libro de trabajo.

```csharp
public string Password { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyPasswordDemo
    {
        public static void Run()
        {
            // Crear LoadOptions y establecer la contraseña
            LoadOptions options = new LoadOptions();
            options.Password = "test";

            // Cargar libro de trabajo protegido con contraseña
            Workbook workbook = new Workbook("protected.xlsx", options);

            // Eliminar la protección con contraseña después de cargar
            workbook.Settings.Password = null;

            // Guardar el libro de trabajo desprotegido
            workbook.Save("unprotected.xlsx");
        }
    }
}
```

### Ver también

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


