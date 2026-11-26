---
title: "Clase CellsFactory"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.CellsFactory. Utilidad para instanciar clases del modelo Cells"
type: docs
url: /es/net/aspose.cells/cellsfactory/
---
## CellsFactory class

Utilidad para instanciar clases del modelo Cells.

```csharp
public class CellsFactory
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [CellsFactory](cellsfactory/)() | El constructor predeterminado. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [CreateStyle](../../aspose.cells/cellsfactory/createstyle/)() | Crea un nuevo estilo. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsFactoryDemo
    {
        public static void CellsFactoryExample()
        {
            // Crear una nueva instancia de CellsFactory
            CellsFactory factory = new CellsFactory();

            // Usar la fábrica para crear un nuevo Style
            Style style = factory.CreateStyle();

            // Personalizar el estilo
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.LightBlue;
            style.Pattern = BackgroundType.Solid;

            // Crear un nuevo libro de trabajo y hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aplicar el estilo a una celda específica
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Styled Cell");
            cell.SetStyle(style);

            // Guardar el libro de trabajo en un archivo
            workbook.Save("CellsFactoryExample.xlsx");
            workbook.Save("CellsFactoryExample.pdf");
            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


