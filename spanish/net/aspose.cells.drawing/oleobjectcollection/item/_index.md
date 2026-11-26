---
title: "OleObjectCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad OleObjectCollection. Obtiene el elemento OleObject en el índice especificado"
type: docs
url: /es/net/aspose.cells.drawing/oleobjectcollection/item/
---
## OleObjectCollection indexer

Obtiene el elemento [`OleObject`](../../oleobject/) en el índice especificado.

```csharp
public OleObject this[int index] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| índice | El índice basado en cero del elemento. |

### Valor de retorno

El elemento en el índice especificado.

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar datos de imagen de muestra
            byte[] binaryImg = File.ReadAllBytes("image1.png");
            
            // Agregar objeto OLE a la primera hoja de cálculo
            int idxOle = workbook.Worksheets[0].OleObjects.Add(0, 0, 60, 60, binaryImg);
            
            // Acceder al objeto OLE usando la propiedad Item
            OleObject objOle = workbook.Worksheets[0].OleObjects[idxOle];
            
            // Establecer propiedades del objeto incrustado
            byte[] binaryXlsx = File.ReadAllBytes("example.xlsx");
            objOle.SetEmbeddedObject(false, binaryXlsx, "SampleFile.xlsx", true, "Excel.Sheet", false);
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
            
            // Verifique el archivo guardado
            Workbook savedWorkbook = new Workbook("output.xlsx");
            Console.WriteLine("OLE Object Source: " + savedWorkbook.Worksheets[0].OleObjects[0].ObjectSourceFullName);
        }
    }
}
```

### Ver también

* class [OleObject](../../oleobject/)
* class [OleObjectCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


