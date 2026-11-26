---
title: "IconFilter.IconSetType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad IconFilter. Obtiene y establece qué conjunto de íconos se usa para este criterio de filtro"
type: docs
url: /es/net/aspose.cells/iconfilter/iconsettype/
---
## IconFilter.IconSetType property

Obtiene y establece qué conjunto de iconos se usa para este criterio de filtro.

```csharp
public IconSetType IconSetType { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IconFilterPropertyIconSetTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Rellene datos de ejemplo
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i * 10);
            }

            // Cree filtro automático
            worksheet.AutoFilter.Range = "A1:A10";
            FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];
            filterColumn.FilterType = FilterType.IconFilter;

            // Obtenga el filtro de iconos
            IconFilter iconFilter = (IconFilter)filterColumn.Filter;

            // Mostrar IconSetType actual (el valor predeterminado es None)
            Console.WriteLine("Current IconSetType: " + iconFilter.IconSetType);

            // Establecer al conjunto de íconos de 3 flechas
            iconFilter.IconSetType = IconSetType.Arrows3;
            iconFilter.IconId = 1; // Show only middle arrow

            // Aplicar formato condicional para visualizar los íconos
            ConditionalFormattingCollection conditionalFormattings = worksheet.ConditionalFormattings;
            int index = conditionalFormattings.Add();
            FormatConditionCollection formatConditionCollection = conditionalFormattings[index];
            int conditionIndex = formatConditionCollection.AddCondition(FormatConditionType.IconSet);
            FormatCondition formatCondition = formatConditionCollection[conditionIndex];
            formatCondition.IconSet.Type = IconSetType.Arrows3;
            
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 9;
            area.StartColumn = 0;
            area.EndColumn = 0;
            formatConditionCollection.AddArea(area);

            // Cambiar al conjunto de íconos de semáforos
            iconFilter.IconSetType = IconSetType.TrafficLights31;
            iconFilter.IconId = 2; // Show only green light

            // Guardar el resultado
            workbook.Save("PropertyIconSetTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [IconSetType](../../iconsettype/)
* class [IconFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


