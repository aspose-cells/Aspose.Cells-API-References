---
title: "Enum SelectionType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enum Aspose.Cells.Drawing.SelectionType. El tipo de selección del cuadro de lista"
type: docs
url: /es/net/aspose.cells.drawing/selectiontype/
---
## SelectionType enumeration

El tipo de selección del cuadro de lista.

```csharp
public enum SelectionType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Single | `0` | Tipo de selección única. |
| Multi | `1` | Tipo de selección múltiple. |
| Extend | `2` | Tipo de selección extendida. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassSelectionTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un cuadro de lista a la hoja de cálculo
            ListBox listBox = worksheet.Shapes.AddListBox(1, 0, 1, 1, 5, 10);

            // Establecer el tipo de selección a Única
            listBox.SelectionType = SelectionType.Single;

            // Agregar elementos al cuadro de lista
            listBox.SetInputRange("A1:A5", false, false);

            // Verificar el tipo de selección
            Console.WriteLine("ListBox SelectionType: " + listBox.SelectionType);

            // Guarda el libro de trabajo
            workbook.Save("SelectionTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


