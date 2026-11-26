---
title: "AutoFilter.AddIconFilter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método AutoFilter. Agrega un filtro de ícono"
type: docs
url: /es/net/aspose.cells/autofilter/addiconfilter/
---
## AutoFilter.AddIconFilter method

Añade un filtro de icono.

```csharp
public void AddIconFilter(int fieldIndex, IconSetType iconSetType, int iconId)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fieldIndex | Int32 | El desplazamiento entero del campo sobre el que desea basar el filtro (desde la izquierda de la lista; el campo más a la izquierda es el campo 0). |
| iconSetType | IconSetType | El tipo de conjunto de íconos. |
| iconId | Int32 | El id del ícono. |

### Observaciones

Solo admite agregar el filtro de ícono. No admite verificar qué fila está visible si el filtro es de ícono.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AutoFilterMethodAddIconFilterWithInt32IconSetTypeInt32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Poblar datos de ejemplo en la columna A
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Values");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);
            worksheet.Cells["A5"].PutValue(40);
            worksheet.Cells["A6"].PutValue(50);
            cell = worksheet.Cells["B1"];
            cell.PutValue("Values2");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);
            worksheet.Cells["B6"].PutValue(50);

            ConditionalFormattingCollection cfs = worksheet.ConditionalFormattings;
            FormatConditionCollection fcs = cfs[cfs.Add()];
            fcs.AddArea(CellArea.CreateCellArea(1, 0, 5, 1));
            FormatCondition fc = fcs[fcs.AddCondition(FormatConditionType.IconSet)];

            // Obtener instancia de autofiltro
            AutoFilter autoFilter = worksheet.AutoFilter;
            
            // Establecer rango de autofiltro (A1:A6) usando startRow, startColumn, endRow
            autoFilter.SetRange(0, 0, 1);

            try
            {
                // Agregar filtro de ícono a la primera columna (fieldIndex: 0)
                // Usando el conjunto de 3 íconos de Semáforos (IconSetType.TrafficLights31)
                // Filtrando por el primer ícono del conjunto (iconId: 0)
                autoFilter.AddIconFilter(0, IconSetType.TrafficLights31, 0);
                
                // Actualizar el filtro para aplicar los cambios
                autoFilter.Refresh();

                Console.WriteLine("Added icon filter to column A showing items with first traffic light icon");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddIconFilter: {ex.Message}");
            }

            // Guardar el libro de trabajo modificado
            workbook.Save("AutoFilterMethodAddIconFilterWithInt32IconSetTypeInt32Demo.xlsx");
        }
    }
}
```

### Ver también

* enum [IconSetType](../../iconsettype/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


