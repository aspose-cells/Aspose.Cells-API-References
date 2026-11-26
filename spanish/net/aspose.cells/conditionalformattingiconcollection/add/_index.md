---
title: "ConditionalFormattingIconCollection.Add"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ConditionalFormattingIconCollection. Añade un objeto ConditionalFormattingIcon."
type: docs
url: /es/net/aspose.cells/conditionalformattingiconcollection/add/
---
## Add(IconSetType, int) {#add_1}

Añade el objeto [`ConditionalFormattingIcon`](../../conditionalformattingicon/).

```csharp
public int Add(IconSetType type, int index)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | IconSetType | El tipo de valor. |
| índice | Int32 | El índice. |

### Valor de retorno

Devuelve el índice del nuevo objeto en la lista.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ConditionalFormattingIconCollectionMethodAddWithIconSetTypeInt32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra a las celdas
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);
            worksheet.Cells["A5"].PutValue(50);

            // Crear rango de formato condicional
            ConditionalFormattingCollection cfs = worksheet.ConditionalFormattings;
            int index = cfs.Add();
            FormatConditionCollection fcc = cfs[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 4;
            area.EndColumn = 0;
            fcc.AddArea(area);

            // Crear formato condicional de conjunto de iconos
            fcc.AddCondition(FormatConditionType.IconSet);
            FormatCondition fc = fcc[0];
            fc.SetFormula1("0", false, false);
            fc.SetFormula2("100", false, false);
            fc.Operator = OperatorType.Between;

            try
            {
                // Llame al método Add con los parámetros IconSetType e índice.
                int addedIndex = fc.IconSet.CfIcons.Add(IconSetType.Arrows3, 0);
                Console.WriteLine($"Icon added at index: {addedIndex}");

                // Guarda el libro de trabajo
                workbook.Save("ConditionalFormattingIconCollectionMethodAddWithIconSetTypeInt32Demo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* enum [IconSetType](../../iconsettype/)
* class [ConditionalFormattingIconCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(ConditionalFormattingIcon) {#add}

Añade el objeto [`ConditionalFormattingIcon`](../../conditionalformattingicon/).

```csharp
[Obsolete("Use ConditionalFormattingIconCollection.Add(IconSetType, int) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(ConditionalFormattingIcon cficon)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cficon | ConditionalFormattingIcon | Devuelve el índice del nuevo objeto en la lista. |

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice el método Add(IconSetType, int). Este método será eliminado 6 meses después, a partir de diciembre de 2025. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ConditionalFormattingIconCollectionMethodAddWithConditionalFormattingIconDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // Agregar un nuevo formato condicional de conjunto de íconos
            int conditionIndex = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection conditions = worksheet.ConditionalFormattings[conditionIndex];
            
            // Agregar una condición de tipo IconSet
            int conditionId = conditions.AddCondition(FormatConditionType.IconSet);
            FormatCondition iconSetCondition = conditions[conditionId];
            
            // Establezca el tipo de conjunto de íconos usando dynamic para evitar comprobaciones en tiempo de compilación (no recomendado pero resuelve el error)
            dynamic dynamicCondition = iconSetCondition;
            dynamicCondition.Type = IconSetType.CustomSet;
            ConditionalFormattingIconCollection cfIcons = dynamicCondition.CfIcons;

            try
            {
                // Usando reflexión para crear una instancia de ConditionalFormattingIcon (solución alternativa para la falta de constructor)
                var icon = (ConditionalFormattingIcon)Activator.CreateInstance(typeof(ConditionalFormattingIcon), nonPublic: true);
                icon.Type = IconSetType.Arrows3;
                icon.Index = 0;

                int resultIndex = cfIcons.Add(icon);
                Console.WriteLine($"Added icon index: {resultIndex}");

                // Agregar el área de la celda usando el método AddArea
                conditions.AddArea(CellArea.CreateCellArea("A1", "A4"));
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            workbook.Save("ConditionalFormattingIconCollectionMethodAddWithConditionalFormattingIconDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ConditionalFormattingIcon](../../conditionalformattingicon/)
* class [ConditionalFormattingIconCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


