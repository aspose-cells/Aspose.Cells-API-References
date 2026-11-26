---
title: "XlsbSaveOptions.LightCellsDataProvider"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad XlsbSaveOptions. El proveedor de datos para guardar el libro de trabajo en modo ligero"
type: docs
url: /es/net/aspose.cells/xlsbsaveoptions/lightcellsdataprovider/
---
## XlsbSaveOptions.LightCellsDataProvider property

El proveedor de datos para guardar el libro de trabajo en modo ligero.

```csharp
public LightCellsDataProvider LightCellsDataProvider { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XlsbSaveOptionsPropertyLightCellsDataProviderDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Poblar algunos datos de muestra
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue($"Data {i}");
            }

            // Crear opciones de guardado XLSB
            XlsbSaveOptions saveOptions = new XlsbSaveOptions();
            saveOptions.LightCellsDataProvider = new CustomLightCellsDataProvider();

            // Guardar el libro de trabajo con LightCellsDataProvider
            using (MemoryStream stream = new MemoryStream())
            {
                workbook.Save(stream, saveOptions);
                
                // Verificar los datos guardados
                stream.Seek(0, SeekOrigin.Begin);
                Workbook savedWorkbook = new Workbook(stream);
                Console.WriteLine("Workbook saved successfully with LightCellsDataProvider");
            }
        }
    }

    public class CustomLightCellsDataProvider : LightCellsDataProvider
    {
        public bool IsGatherString()
        {
            return true;
        }

        public int NextCell()
        {
            // Implementar la lógica de iteración de celdas aquí
            return -1; // Return -1 when no more cells
        }

        public int NextRow()
        {
            // Implementar la lógica de iteración de filas aquí
            return -1; // Return -1 when no more rows
        }

        public void StartCell(Cell cell)
        {
            // Implementar la lógica de procesamiento de celdas aquí
        }

        public void StartRow(Row row)
        {
            // Implementar la lógica de procesamiento de filas aquí
        }

        public bool StartSheet(int sheetIndex)
        {
            // Implementar la lógica de procesamiento de hojas aquí
            return true; // Return true to process the sheet
        }
    }
}
```

### Ver también

* interface [LightCellsDataProvider](../../lightcellsdataprovider/)
* class [XlsbSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


