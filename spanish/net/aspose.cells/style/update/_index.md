---
title: "Style.Update"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Style. Aplica el estilo con nombre a los estilos de las celdas que usan este estilo con nombre. Funciona como hacer clic en el botón aceptar después de terminar de modificar el estilo. Sólo se aplica al estilo con nombre"
type: docs
url: /es/net/aspose.cells/style/update/
---
## Style.Update method

Aplica el estilo nombrado a los estilos de las celdas que usan este estilo nombrado. Funciona como hacer clic en el botón \"ok\" después de haber terminado de modificar el estilo. Solo se aplica al estilo nombrado.

```csharp
public void Update()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleMethodUpdateDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear un estilo
            Style style = workbook.CreateStyle();
            style.Number = 3; // Set to Percent format
            
            // Aplicar el estilo a la celda A1
            worksheet.Cells["A1"].SetStyle(style);
            
            // Modificar el estilo
            style.Number = 4; // Change to Currency format
            
            // Actualizar los cambios del estilo
            style.Update();
            
            // Verificar que el estilo se haya actualizado
            Console.WriteLine("Cell A1 Number Format: " + worksheet.Cells["A1"].GetStyle().Number);
        }
    }
}
```

### Ver también

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


