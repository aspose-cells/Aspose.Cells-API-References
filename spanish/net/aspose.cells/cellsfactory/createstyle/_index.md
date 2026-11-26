---
title: "CellsFactory.CreateStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método de CellsFactory. Crea un nuevo estilo"
type: docs
url: /es/net/aspose.cells/cellsfactory/createstyle/
---
## CellsFactory.CreateStyle method

Crea un nuevo estilo.

```csharp
public Style CreateStyle()
```

### Valor de retorno

Devuelve un objeto de estilo.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class CellsFactoryMethodCreateStyleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Crear un estilo usando CellsFactory
            Style style = new CellsFactory().CreateStyle();
            
            // Establecer propiedades de borde para el estilo
            style.SetBorder(BorderType.BottomBorder, CellBorderType.Thick, Color.Black);
            
            // Aplicar el estilo a una celda
            workbook.Worksheets[0].Cells["A1"].Value = "Hello World";
            workbook.Worksheets[0].Cells["A1"].SetStyle(style);
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [Style](../../style/)
* class [CellsFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


