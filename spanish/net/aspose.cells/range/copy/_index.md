---
title: "Range.Copy"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Range. Copiar el rango con opciones de pegado especial"
type: docs
url: /es/net/aspose.cells/range/copy/
---
## Copy(Range, PasteOptions) {#copy_1}

Copiando el rango con opciones de pegado especial.

```csharp
public void Copy(Range range, PasteOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rango | Rango | El rango de origen. |
| opciones | PasteOptions | Las opciones de pegado especial. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodCopyWithRangePasteOptionsDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Crear datos de muestra en el rango de origen
            for (int i = 0; i < 5; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    sheet.Cells[i, j].PutValue($"Data {i},{j}");
                }
            }

            // Crear rangos con tipo totalmente calificado
            Aspose.Cells.Range source = sheet.Cells.CreateRange(0, 0, 5, 5);
            Aspose.Cells.Range destination = sheet.Cells.CreateRange(6, 0, 5, 5);

            // Establecer opciones de pegado
            PasteOptions options = new PasteOptions();
            options.PasteType = PasteType.All;

            // Copiar con opciones de pegado
            destination.Copy(source, options);

            wb.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [PasteOptions](../../pasteoptions/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Copy(Range) {#copy}

Copia datos (incluidas fórmulas), formato, objetos de dibujo, etc., de un rango de origen.

```csharp
public void Copy(Range range)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| range | Range | Objeto [`Range`](../) de origen. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodCopyWithRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Crea rangos de origen y de destino
            Aspose.Cells.Range sourceRange = cells.CreateRange("A1:A5");
            Aspose.Cells.Range destRange = cells.CreateRange("A6:A10");
            
            // Rellenar el rango de origen con datos de muestra
            for (int i = 0; i < 5; i++)
            {
                sourceRange[i, 0].PutValue($"Data {i + 1}");
            }
            
            // Copiar el rango de origen al destino
            sourceRange.Copy(destRange);
            
            workbook.Save("RangeCopyDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


