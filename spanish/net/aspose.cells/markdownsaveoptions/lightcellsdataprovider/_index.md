---
title: "MarkdownSaveOptions.LightCellsDataProvider"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad MarkdownSaveOptions. El proveedor de datos que suministra los datos de celdas para guardar el libro de trabajo en modo ligero"
type: docs
url: /es/net/aspose.cells/markdownsaveoptions/lightcellsdataprovider/
---
## MarkdownSaveOptions.LightCellsDataProvider property

El proveedor de datos para proporcionar datos de celdas al guardar el libro de trabajo en modo ligero.

```csharp
public LightCellsDataProvider LightCellsDataProvider { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections.Generic;

    public class MarkdownSaveOptionsPropertyLightCellsDataProviderDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Poblar algunos datos de muestra
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].Value = "Item " + (i + 1);
                worksheet.Cells[i, 1].Value = i + 1;
            }

            // Crear LightCellsDataProvider personalizado
            var dataProvider = new CustomLightCellsDataProvider();

            // Crear MarkdownSaveOptions
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();
            
            // Mostrar valor actual (debería ser null inicialmente)
            Console.WriteLine("Current LightCellsDataProvider value: " + (saveOptions.LightCellsDataProvider == null ? "null" : "set"));

            // Establecer el proveedor de datos personalizado
            saveOptions.LightCellsDataProvider = dataProvider;

            // Guardar con el proveedor de datos personalizado
            workbook.Save("LightCellsDataProviderDemo.md", saveOptions);
        }
    }

    public class CustomLightCellsDataProvider : LightCellsDataProvider
    {
        private List<string> items = new List<string> { "Apple", "Banana", "Cherry", "Date", "Elderberry" };
        private List<double> values = new List<double> { 1.99, 0.99, 2.99, 3.49, 4.99 };
        private int currentRow = -1;

        public bool StartSheet(int sheetIndex)
        {
            // Procesar solo la primera hoja
            return sheetIndex == 0;
        }

        public int NextRow()
        {
            currentRow++;
            return currentRow < items.Count ? currentRow : -1;
        }

        public void StartRow(Row row)
        {
            // Establecer la altura de la fila si es necesario
            row.Height = 15;
        }

        public int NextCell()
        {
            if (currentRow == -1)
            {
                // Fila de encabezado
                return currentRow < 2 ? currentRow + 1 : -1;
            }
            else
            {
                return currentRow < 2 ? currentRow + 1 : -1;
            }
        }

        public void StartCell(Cell cell)
        {
            if (currentRow == -1)
            {
                // Encabezado
                if (cell.Column == 0)
                    cell.Value = "Product";
                else if (cell.Column == 1)
                    cell.Value = "Price";
            }
            else
            {
                // Datos
                if (cell.Column == 0)
                    cell.Value = items[currentRow];
                else if (cell.Column == 1)
                    cell.Value = values[currentRow];
            }
        }

        public bool IsGatherString()
        {
            return false;
        }
    }
}
```

### Ver también

* interface [LightCellsDataProvider](../../lightcellsdataprovider/)
* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


