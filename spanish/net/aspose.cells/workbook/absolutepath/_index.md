---
title: "Workbook.AbsolutePath"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Workbook. Obtiene y establece la ruta absoluta del archivo"
type: docs
url: /es/net/aspose.cells/workbook/absolutepath/
---
## Workbook.AbsolutePath property

Obtiene y establece la ruta absoluta del archivo.

```csharp
public string AbsolutePath { get; set; }
```

### Observaciones

Solo se usa para enlaces externos.

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyAbsolutePathDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook sourceBook = new Workbook();
            
            // Agregar algunas hojas de cálculo
            sourceBook.Worksheets.Add("Sheet1");
            sourceBook.Worksheets.Add("Sheet2");

            // Guarde el workbook para obtener una ruta física
            string sourcePath = Path.GetFullPath("output");
            if (!Directory.Exists(sourcePath))
            {
                Directory.CreateDirectory(sourcePath);
            }
            string sourceFilePath = Path.Combine(sourcePath, "example.xlsx");
            sourceBook.Save(sourceFilePath);

            // Reabra el workbook para demostrar AbsolutePath
            Workbook reopenedBook = new Workbook(sourceFilePath);
            
            // Utilice la propiedad AbsolutePath para construir la ruta completa
            string pathToBook = Path.Combine(reopenedBook.AbsolutePath, reopenedBook.FileName);
            Console.WriteLine("Full path to workbook: " + pathToBook);

            // Agregar hipervínculos usando la ruta
            SetHyperlink(reopenedBook.Worksheets[0], 0, pathToBook, reopenedBook.Worksheets[0].Name, "A1");
            SetHyperlink(reopenedBook.Worksheets[0], 1, pathToBook, reopenedBook.Worksheets[1].Name, "B1");

            // Guardar el libro de trabajo modificado
            string destPath = Path.Combine(sourcePath, "modified_example.xlsx");
            reopenedBook.Save(destPath);
        }

        private static void SetHyperlink(Worksheet sheet, int linkIndex, string path, string sheetName, string cellRef)
        {
            HyperlinkCollection hyperlinks = sheet.Hyperlinks;
            hyperlinks.Add(cellRef, 1, 1, path + "#" + sheetName + "!A1");
        }
    }
}
```

### Ver también

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


