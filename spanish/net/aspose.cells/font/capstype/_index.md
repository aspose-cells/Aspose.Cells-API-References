---
title: "Font.CapsType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Font. Obtiene y establece el tipo de mayúsculas del texto"
type: docs
url: /es/net/aspose.cells/font/capstype/
---
## Font.CapsType property

Obtiene y establece el tipo de mayúsculas del texto.

```csharp
[Obsolete("Use TextOptions.CapsType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public TextCapsType CapsType { get; set; }
```

### Observaciones

Solo para las fuentes de Shapes o Charts. NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad [`CapsType`](../../../aspose.cells.drawing.texts/textoptions/capstype/) . Esta propiedad será eliminada 12 meses después a partir de enero de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyCapsTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("sample text");

            Style style = cell.GetStyle();
            style.Font.CapsType = TextCapsType.All;
            cell.SetStyle(style);

            workbook.Save("FontCapsTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [TextCapsType](../../textcapstype/)
* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


