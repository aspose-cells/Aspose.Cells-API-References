---
title: "Cells.Find"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Encuentra la celda que contiene el objeto de entrada"
type: docs
url: /es/net/aspose.cells/cells/find/
---
## Find(object, Cell) {#find}

Encuentra la celda que contiene el objeto de entrada.

```csharp
public Cell Find(object what, Cell previousCell)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| qué | Objeto | El objeto a buscar. El tipo debe ser int,double,DateTime,string,bool. |
| previousCell | Celda | Celda anterior con el mismo objeto. Este parámetro puede establecerse en null si se busca desde el inicio. |

### Valor de retorno

Objeto de celda.

### Observaciones

Devuelve null (Nothing) si no se encuentra ninguna celda.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodFindWithObjectCellDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(2.5);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(1.8);
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B4"].PutValue(1.2);

            // Buscar la celda que contiene "Orange"
            Cell searchCell = null;
            Cell foundCell = worksheet.Cells.Find("Orange", searchCell);

            if (foundCell != null)
            {
                Console.WriteLine("Found 'Orange' at: " + foundCell.Name);
                
                // Crear y aplicar un estilo a la celda encontrada
                Style style = workbook.CreateStyle();
                style.Font.Color = System.Drawing.Color.Red;
                style.Font.IsBold = true;
                foundCell.SetStyle(style);
            }

            // Guarda el libro de trabajo
            workbook.Save("FindMethodDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Find(object, Cell, FindOptions) {#find_1}

Encuentra la celda que contiene el objeto de entrada.

```csharp
public Cell Find(object what, Cell previousCell, FindOptions findOptions)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| qué | Objeto | El objeto a buscar. El tipo debe ser int,double,DateTime,string,bool. |
| previousCell | Celda | Celda anterior con el mismo objeto. Este parámetro puede establecerse en null si se busca desde el inicio. |
| findOptions | FindOptions | Opciones de búsqueda |

### Valor de retorno

Objeto de celda.

### Observaciones

Devuelve null (Nothing) si no se encuentra ninguna celda.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodFindWithObjectCellFindOptionsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer datos de muestra
            worksheet.Cells["A1"].PutValue("abc");
            worksheet.Cells["A2"].PutValue("def");
            worksheet.Cells["A3"].PutValue("abc ");
            
            // Crear opciones de búsqueda
            FindOptions options = new FindOptions();
            options.LookInType = LookInType.Values;
            options.LookAtType = LookAtType.Contains;
            
            // Buscar celda con valor "abc "
            Cell foundCell = worksheet.Cells.Find("abc ", null, options);
            
            Console.WriteLine("Found cell: " + (foundCell != null ? foundCell.Name : "null"));
        }
    }
}
```

### Ver también

* class [Cell](../../cell/)
* class [FindOptions](../../findoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


