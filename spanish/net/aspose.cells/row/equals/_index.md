---
title: "Row.Equals"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Row. Comprueba si este objeto se refiere a la misma fila que otro"
type: docs
url: /es/net/aspose.cells/row/equals/
---
## Equals(object) {#equals_1}

Comprueba si este objeto se refiere a la misma fila que otro.

```csharp
public override bool Equals(object obj)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| obj | Objeto | otro objeto |

### Valor de retorno

verdadero si dos objetos se refieren a la misma fila.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RowMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear dos filas para comparar
            Row row1 = worksheet.Cells.Rows[0];
            Row row2 = worksheet.Cells.Rows[1];
            
            // Establecer algunas propiedades para que las filas sean diferentes
            row1.Height = 20;
            row2.Height = 25;
            
            try
            {
                // Llamar al método Equals con el parámetro Object
                bool result1 = row1.Equals((object)row2);
                Console.WriteLine($"Comparing row1 with row2: {result1}");
                
                // Comparar row1 consigo mismo
                bool result2 = row1.Equals((object)row1);
                Console.WriteLine($"Comparing row1 with itself: {result2}");
                
                // Comparar con null
                bool result3 = row1.Equals((object)null);
                Console.WriteLine($"Comparing row1 with null: {result3}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }
            
            workbook.Save("RowMethodEqualsWithObjectDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Equals(Row) {#equals}

Comprueba si este objeto se refiere a la misma fila que otro objeto de fila.

```csharp
public bool Equals(Row row)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | Row | otro objeto de fila |

### Valor de retorno

verdadero si dos objetos de fila se refieren a la misma fila.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RowMethodEqualsWithRowDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear dos filas para comparar
            Row row1 = worksheet.Cells.Rows[0];
            Row row2 = worksheet.Cells.Rows[1];

            // Establecer algunas propiedades para que las filas sean diferentes
            row1.Height = 20;
            row2.Height = 25;
            row1.IsHidden = false;
            row2.IsHidden = true;

            try
            {
                // Llame al método Equals para comparar las filas
                bool areEqual = row1.Equals(row2);

                // Mostrar el resultado
                Console.WriteLine($"Are rows equal? {areEqual}");

                // Cree otra fila con las mismas propiedades que row1
                Row row3 = worksheet.Cells.Rows[2];
                row3.Height = row1.Height;
                row3.IsHidden = row1.IsHidden;

                // Compare row1 con row3 (debe ser igual)
                bool areEqual2 = row1.Equals(row3);
                Console.WriteLine($"Are rows equal after matching properties? {areEqual2}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Guarda el libro de trabajo
            workbook.Save("RowEqualsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


