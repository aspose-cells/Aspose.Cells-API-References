---
title: "WorksheetCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorksheetCollection. Obtiene el elemento Worksheet en el índice especificado"
type: docs
url: /es/net/aspose.cells/worksheetcollection/item/
---
## WorksheetCollection indexer (1 of 2)

Obtiene el elemento [`Worksheet`](../../worksheet/) en el índice especificado.

```csharp
public Worksheet this[int index] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| índice | El índice basado en cero del elemento. |

### Valor de retorno

El elemento en el índice especificado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Usando la propiedad Item para acceder a la celda
            Cell cell = cells[0, 0];
            cell.Formula = "=SUM(1, 2, 3)";
            
            workbook.CalculateFormula();
            Console.WriteLine("Cell value: " + cell.IntValue);
        }
    }
}
```

### Ver también

* class [Worksheet](../../worksheet/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## WorksheetCollection indexer (2 of 2)

Obtiene el elemento [`Worksheet`](../../worksheet/) con el nombre especificado.

```csharp
public Worksheet this[string sheetName] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| sheetName | Nombre de la hoja de cálculo |

### Valor de retorno

El elemento con el nombre especificado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a las hojas de cálculo usando la propiedad Item por índice y nombre
            Worksheet sheet1 = workbook.Worksheets[0];
            sheet1.Name = "FirstSheet";
            
            Worksheet sheet2 = workbook.Worksheets.Add("SecondSheet");
            
            // Acceder a la hoja de cálculo por nombre usando la propiedad Item
            Worksheet accessedSheet = workbook.Worksheets["FirstSheet"];
            
            // Agregar datos para demostrar el acceso a la hoja de cálculo
            Cells cells = accessedSheet.Cells;
            cells["A1"].PutValue("Worksheet accessed successfully!");
            cells["A2"].PutValue(DateTime.Now.ToString());
            
            // Insertar una columna en la segunda hoja
            workbook.Worksheets["SecondSheet"].Cells.InsertColumn(1);
            
            // Guarda el libro de trabajo
            workbook.Save("WorksheetCollectionItemDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Worksheet](../../worksheet/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


