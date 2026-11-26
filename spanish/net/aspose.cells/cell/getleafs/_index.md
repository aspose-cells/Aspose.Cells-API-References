---
title: "Cell.GetLeafs"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cell. Obtenga todas las celdas que hacen referencia a esta celda directamente y que deben actualizarse cuando esta celda se modifica"
type: docs
url: /es/net/aspose.cells/cell/getleafs/
---
## GetLeafs() {#getleafs}

Obtenga todas las celdas que hacen referencia a esta celda directamente y que deben actualizarse cuando esta celda se modifica.

```csharp
[Obsolete("Use GetDependentsInCalculation(bool) instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public IEnumerator GetLeafs()
```

### Valor de retorno

Enumerador para enumerar todos los dependientes (Cell)

### Observaciones

NOTA: Esta clase está ahora obsoleta. En su lugar, utilice Cell.GetDependentsInCalculation(bool) para obtener todos los dependientes en la cadena de cálculo. Esta propiedad será eliminada 12 meses después a partir de mayo de 2022. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class CellMethodGetLeafsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue algunos datos y fórmulas para crear dependencias
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["B1"].Formula = "=A1+A2";
            worksheet.Cells["C1"].Formula = "=B1*2";

            try
            {
                // Obtenga la celda que tiene dependientes
                Cell cell = worksheet.Cells["B1"];

                // Llame a GetLeafs para obtener todas las celdas que hacen referencia a esta celda directamente
                IEnumerator leafs = cell.GetLeafs();

                Console.WriteLine("Cells that directly reference B1:");
                while (leafs.MoveNext())
                {
                    Cell leafCell = leafs.Current as Cell;
                    if (leafCell != null)
                    {
                        Console.WriteLine($"Cell: {leafCell.Name}, Formula: {leafCell.Formula}");
                    }
                }

                // Guarda el libro de trabajo
                workbook.Save("GetLeafsDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetLeafs: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetLeafs(bool) {#getleafs_1}

Obtenga todas las celdas que se actualizarán cuando esta celda se modifique.

```csharp
[Obsolete("Use GetDependentsInCalculation(bool) instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public IEnumerator GetLeafs(bool recursive)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| recursivo | Booleano | Devuelve si esas hojas no hacen referencia a esta celda directamente, sino a otras hojas de esta celda |

### Valor de retorno

Enumerador para enumerar todos los dependientes (Cell)

### Observaciones

NOTA: Esta clase está ahora obsoleta. En su lugar, utilice Cell.GetDependentsInCalculation(bool) para obtener todos los dependientes en la cadena de cálculo. Esta propiedad será eliminada 12 meses después a partir de mayo de 2022. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class CellMethodGetLeafsWithBooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue algunos datos con fórmulas para crear dependencias
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["A2"].Value = 20;
            worksheet.Cells["B1"].Formula = "=A1+A2";
            worksheet.Cells["C1"].Formula = "=B1*2";

            try
            {
                // Obtenga la celda que tiene dependientes
                Cell cell = worksheet.Cells["A1"];

                // Llame a GetLeafs con el parámetro recursivo establecido en true
                IEnumerator leafs = cell.GetLeafs(true);

                // Muestra los resultados
                Console.WriteLine("Leaf cells found:");
                while (leafs.MoveNext())
                {
                    Cell leaf = (Cell)leafs.Current;
                    Console.WriteLine($"Cell: {leaf.Name}, Value: {leaf.Value}");
                }

                // Guarda el libro de trabajo
                workbook.Save("GetLeafsDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetLeafs: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


