---
title: "IconFilter.IconId"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad IconFilter. Obtiene y establece el índice basado en cero de un ícono en un conjunto de íconos"
type: docs
url: /es/net/aspose.cells/iconfilter/iconid/
---
## IconFilter.IconId property

Obtiene y establece el índice basado en cero de un icono en un conjunto de iconos.

```csharp
public int IconId { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IconFilterPropertyIconIdDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Rellene datos de ejemplo
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i + 1);
            }

            // Aplicar formato condicional de conjunto de íconos
            ConditionalFormattingCollection conditionalFormattings = worksheet.ConditionalFormattings;
            int index = conditionalFormattings.Add();
            FormatConditionCollection formatConditionCollection = conditionalFormattings[index];
            int conditionIndex = formatConditionCollection.AddCondition(FormatConditionType.IconSet);
            FormatCondition formatCondition = formatConditionCollection[conditionIndex];
            formatCondition.IconSet.Type = IconSetType.TrafficLights31;
            
            // Establecer rango usando CellArea
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 9;
            area.StartColumn = 0;
            area.EndColumn = 0;
            formatConditionCollection.AddArea(area);

            // Crear filtro automático con filtro de íconos
            worksheet.AutoFilter.Range = "A1:A10";
            FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];
            filterColumn.FilterType = FilterType.IconFilter;
            
            // Obtener filtro existente en lugar de crear una nueva instancia
            IconFilter iconFilter = (IconFilter)filterColumn.Filter;
            iconFilter.IconSetType = IconSetType.TrafficLights31;
            iconFilter.IconId = 0;

            Console.WriteLine("Current IconId value: " + iconFilter.IconId);

            // Modificar IconId para filtrar diferentes íconos
            iconFilter.IconId = 1;

            workbook.Save("PropertyIconIdDemo.xlsx");
        }
    }
}
```

### Ver también

* class [IconFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


