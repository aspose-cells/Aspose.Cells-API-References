---
title: "ICellsDataTable.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ICellsDataTable. Obtiene los datos almacenados en la columna especificada por índice"
type: docs
url: /es/net/aspose.cells/icellsdatatable/item/
---
## ICellsDataTable indexer (1 of 2)

Obtiene los datos almacenados en la columna especificada por índice.

```csharp
public object this[int columnIndex] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| columnIndex | El índice basado en cero de la columna. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ICellsDataTablePropertyItemDemo
    {
        public static void Run()
        {
            // Crear ICellsDataTable personalizado con datos de ejemplo
            ICellsDataTable dataTable = new SampleDataTable();

            // Restablecer la posición del cursor
            dataTable.BeforeFirst();

            Console.WriteLine("Reading data using Item property:");
            while (dataTable.Next())
            {
                // Acceder a los valores por índice de columna
                Console.WriteLine($"Product: {dataTable[0]}, Price: {dataTable[1]}, Stock: {dataTable[2]}");

                // Acceder a los valores por nombre de columna
                Console.WriteLine($"Product: {dataTable["Product"]}, Price: {dataTable["Price"]}, Stock: {dataTable["Stock"]}\n");
            }
        }
    }

    internal class SampleDataTable : ICellsDataTable
    {
        private readonly string[] columns = { "Product", "Price", "Stock" };
        private readonly object[][] data = 
        {
            new object[] { "Laptop", 999.99, 15 },
            new object[] { "Phone", 699.99, 25 },
            new object[] { "Tablet", 299.99, 50 }
        };
        private int currentRow = -1;

        public string[] Columns => columns;
        public int Count => data.Length;

        public object this[int columnIndex] => data[currentRow][columnIndex];
        public object this[string columnName] => data[currentRow][Array.IndexOf(columns, columnName)];

        public void BeforeFirst() => currentRow = -1;
        public bool Next() => ++currentRow < data.Length;
    }
}
```

### Ver también

* interface [ICellsDataTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ICellsDataTable indexer (2 of 2)

Obtiene los datos almacenados en la columna especificada por nombre de columna.

```csharp
public object this[string columnName] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| columnName | El nombre de la columna. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ICellsDataTablePropertyItemDemo1
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Poblar datos de ejemplo en celdas
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(999.99);
            worksheet.Cells["A3"].PutValue("Phone");
            worksheet.Cells["B3"].PutValue(499.99);

            // Exportar rango de datos a ICellsDataTable con conversión explícita
            ICellsDataTable dataTable = (ICellsDataTable)worksheet.Cells.ExportDataTable(0, 0, 3, 2);

            // Moverse antes del primer registro
            dataTable.BeforeFirst();

            Console.WriteLine("Reading data table values:");
            while (dataTable.Next())
            {
                // Acceder a la propiedad Item usando nombres de columna (indexador)
                string product = dataTable["Product"].ToString();
                double price = Convert.ToDouble(dataTable["Price"]);

                Console.WriteLine($"Item[Product]: {product}, Item[Price]: {price}");
            }

            // Guarda el libro de trabajo
            workbook.Save("ItemPropertyDemo.xlsx");
        }
    }
}
```

### Ver también

* interface [ICellsDataTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


