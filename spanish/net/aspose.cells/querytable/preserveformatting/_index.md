---
title: "QueryTable.PreserveFormatting"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad QueryTable. Devuelve o establece PreserveFormatting del objeto"
type: docs
url: /es/net/aspose.cells/querytable/preserveformatting/
---
## QueryTable.PreserveFormatting property

Devuelve o establece el PreserveFormatting del objeto.

```csharp
public bool PreserveFormatting { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class QueryTablePropertyPreserveFormattingDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo y formato
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["A3"].PutValue("Phone");
            worksheet.Cells["B3"].PutValue(800);

            // Aplicar formato al rango de datos
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.LightBlue;
            style.Pattern = BackgroundType.Solid;
            
            // Aplicar estilo a cada celda en el rango
            worksheet.Cells["A1"].SetStyle(style);
            worksheet.Cells["B1"].SetStyle(style);

            // Crear una tabla de consulta (simulada ya que la creación real requiere una fuente de datos externa)
            // En uso real, crearías esto a partir de una conexión externa
            QueryTable queryTable = worksheet.QueryTables[0];

            // Mostrar el valor actual de PreserveFormatting
            Console.WriteLine("Initial PreserveFormatting value: " + queryTable.PreserveFormatting);

            // Establecer PreserveFormatting a false (no preservará el formato existente durante la actualización)
            queryTable.PreserveFormatting = false;
            Console.WriteLine("PreserveFormatting set to: " + queryTable.PreserveFormatting);

            // Simular la actualización de la tabla de consulta (normalmente borraría el formato cuando PreserveFormatting es false)
            // En un escenario real, esto ocurriría cuando la tabla de consulta actualiza sus datos
            Console.WriteLine("After refresh with PreserveFormatting=false, formatting would be lost");

            // Establecer PreserveFormatting a true
            queryTable.PreserveFormatting = true;
            Console.WriteLine("PreserveFormatting set to: " + queryTable.PreserveFormatting);

            // Simular la actualización nuevamente (ahora preservará el formato)
            Console.WriteLine("After refresh with PreserveFormatting=true, formatting is preserved");

            // Guarda el libro de trabajo
            workbook.Save("QueryTablePreserveFormattingDemo.xlsx");
        }
    }
}
```

### Ver también

* class [QueryTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


