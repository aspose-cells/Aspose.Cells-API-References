---
title: "Font.CapsType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Font. Ottiene e imposta il tipo di maiuscole del testo"
type: docs
url: /it/net/aspose.cells/font/capstype/
---
## Font.CapsType property

Ottiene e imposta il tipo di maiuscole del testo.

```csharp
[Obsolete("Use TextOptions.CapsType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public TextCapsType CapsType { get; set; }
```

### Osservazioni

Solo per i caratteri di Forme o Grafici. NOTA: questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà [`CapsType`](../../../aspose.cells.drawing.texts/textoptions/capstype/). Questa proprietà sarà rimossa 12 mesi dopo, a partire da gennaio 2026. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

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

### Vedi anche

* enum [TextCapsType](../../textcapstype/)
* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


