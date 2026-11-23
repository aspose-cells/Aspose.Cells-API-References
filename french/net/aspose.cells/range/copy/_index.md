---
title: "Range.Copy"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Range. Copier la plage avec les options de collage spécial"
type: docs
url: /fr/net/aspose.cells/range/copy/
---
## Copy(Range, PasteOptions) {#copy_1}

Copie la plage avec les options de collage spécial.

```csharp
public void Copy(Range range, PasteOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| plage | Plage | La plage source. |
| options | PasteOptions | Les options de collage spécial. |

### Exemples

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
            
            // Créer des données d'exemple dans la plage source
            for (int i = 0; i < 5; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    sheet.Cells[i, j].PutValue($"Data {i},{j}");
                }
            }

            // Créer des plages avec le type entièrement qualifié
            Aspose.Cells.Range source = sheet.Cells.CreateRange(0, 0, 5, 5);
            Aspose.Cells.Range destination = sheet.Cells.CreateRange(6, 0, 5, 5);

            // Définir les options de collage
            PasteOptions options = new PasteOptions();
            options.PasteType = PasteType.All;

            // Copier avec les options de collage
            destination.Copy(source, options);

            wb.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [PasteOptions](../../pasteoptions/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Copy(Range) {#copy}

Copie les données (y compris les formules), le formatage, les objets de dessin, etc. depuis une plage source.

```csharp
public void Copy(Range range)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| range | Range | Objet source [`Range`](../). |

### Exemples

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
            
            // Créez les plages source et destination
            Aspose.Cells.Range sourceRange = cells.CreateRange("A1:A5");
            Aspose.Cells.Range destRange = cells.CreateRange("A6:A10");
            
            // Remplir la plage source avec des données d'exemple
            for (int i = 0; i < 5; i++)
            {
                sourceRange[i, 0].PutValue($"Data {i + 1}");
            }
            
            // Copier la plage source vers la destination
            sourceRange.Copy(destRange);
            
            workbook.Save("RangeCopyDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


