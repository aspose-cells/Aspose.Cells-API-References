---
title: "OdsCellField.FieldType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad OdsCellField. Obtiene y establece el tipo del campo"
type: docs
url: /es/net/aspose.cells.ods/odscellfield/fieldtype/
---
## OdsCellField.FieldType property

Obtiene y establece el tipo del campo.

```csharp
public OdsCellFieldType FieldType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsCellFieldPropertyFieldTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar campos de celda ODS con diferentes tipos de campo y cadenas de formato
            sheet.Cells.OdsCellFields.Add(0, 0, OdsCellFieldType.Title, "Title Format");
            sheet.Cells.OdsCellFields.Add(1, 0, OdsCellFieldType.SheetName, "SheetName Format");

            // Demostrar el uso de la propiedad FieldType
            Console.WriteLine("Field at (0,0) type: " + sheet.Cells.OdsCellFields[0].FieldType);
            Console.WriteLine("Field at (1,0) type: " + sheet.Cells.OdsCellFields[1].FieldType);

            // Guarde y vuelva a cargar para demostrar la persistencia
            workbook.Save("output.ods");
            workbook = new Workbook("output.ods");
            sheet = workbook.Worksheets[0];

            // Verificar FieldType después de recargar
            Console.WriteLine("After reload - Field at (0,0) type: " + sheet.Cells.OdsCellFields[0].FieldType);
            Console.WriteLine("After reload - Field at (1,0) type: " + sheet.Cells.OdsCellFields[1].FieldType);
        }
    }
}
```

### Ver también

* enum [OdsCellFieldType](../../odscellfieldtype/)
* class [OdsCellField](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


