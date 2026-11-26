---
title: "ConditionalFormattingCollection.RemoveArea"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ConditionalFormattingCollection. Elimina todo el formato condicional en el rango"
type: docs
url: /es/net/aspose.cells/conditionalformattingcollection/removearea/
---
## ConditionalFormattingCollection.RemoveArea method

Elimina todo el formato condicional en el rango.

```csharp
public void RemoveArea(int startRow, int startColumn, int totalRows, int totalColumns)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startRow | Int32 | La fila inicial del rango. |
| startColumn | Int32 | La columna inicial del rango. |
| totalRows | Int32 | El número de filas del rango. |
| totalColumns | Int32 | El número de columnas del rango. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ConditionalFormattingCollectionMethodRemoveAreaWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Obtener la colección de formato condicional
            ConditionalFormattingCollection cfc = worksheet.ConditionalFormattings;

            // Agregar algunas reglas de formato condicional
            int index = cfc.Add();
            FormatConditionCollection fcc = cfc[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 5;
            area.EndColumn = 5;
            fcc.AddArea(area);

            try
            {
                // Llamar a RemoveArea con los parámetros (Int32, Int32, Int32, Int32)
                cfc.RemoveArea(0, 0, 3, 3);

                Console.WriteLine("Conditional formatting removed from area (0,0,3,3)");
                
                // Verificar el efecto comprobando el recuento (esto sería 0 si se eliminó todo el formato)
                Console.WriteLine($"Remaining conditional formatting areas: {fcc.RangeCount}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveArea method: {ex.Message}");
            }
            
            // Guardar el resultado
            workbook.Save("RemoveAreaWithInt32Demo.xlsx");
        }
    }
}
```

### Ver también

* class [ConditionalFormattingCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


