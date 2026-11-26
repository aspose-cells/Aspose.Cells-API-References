---
title: "SaveOptions.ClearData"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SaveOptions. Dejar el libro de trabajo vacío después de guardar el archivo"
type: docs
url: /es/net/aspose.cells/saveoptions/cleardata/
---
## SaveOptions.ClearData property

Dejar el libro de trabajo vacío después de guardar el archivo.

```csharp
public bool ClearData { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyClearDataDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de prueba
            worksheet.Cells["A1"].PutValue("Tabelle1");
            worksheet.Cells["B3"].PutValue(3);

            // Configurar opciones de guardado con ClearData = false
            TxtSaveOptions saveOptions = new TxtSaveOptions();
            saveOptions.ClearData = false;
            saveOptions.Separator = ',';

            // Guarda el libro de trabajo
            string outputPath = "output_with_cleardata_false.csv";
            workbook.Save(outputPath, saveOptions);

            // Recargar para verificar que los datos se conservaron
            Workbook loadedWorkbook = new Workbook(outputPath);
            Cells cells = loadedWorkbook.Worksheets[0].Cells;
            
            Console.WriteLine("A1 value: " + cells["A1"].StringValue);
            Console.WriteLine("B3 value: " + cells["B3"].IntValue);
        }
    }
}
```

### Ver también

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


