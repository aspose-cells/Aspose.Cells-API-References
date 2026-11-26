---
title: "Enum TextCrossType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enum Aspose.Cells.TextCrossType. Enumera el tipo de visualización de texto cuando el ancho del texto es mayor que el ancho de la celda"
type: docs
url: /es/net/aspose.cells/textcrosstype/
---
## TextCrossType enumeration

Enumera el tipo de visualización de texto cuando el ancho del texto es mayor que el ancho de la celda.

```csharp
public enum TextCrossType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Default | `1` | Mostrar texto como en Microsoft Excel. |
| CrossKeep | `2` | Mostrar todo el texto cruzando otras celdas y mantener el texto de las celdas cruzadas. |
| CrossOverride | `3` | Mostrar todo el texto cruzando otras celdas y sobrescribir el texto de las celdas cruzadas. |
| StrictInCell | `4` | Mostrar solo el texto dentro del ancho de la celda. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class CellsClassTextCrossTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer texto de muestra en una celda que podría desbordarse
            worksheet.Cells["A1"].PutValue("This is a long text that might overflow the cell");
            
            // Crear opciones de imagen o impresión
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            
            // Demostrar diferentes configuraciones de TextCrossType
            options.TextCrossType = TextCrossType.Default;
            SaveToImage(workbook, options, "TextCrossType_Default.png");
            
            options.TextCrossType = TextCrossType.CrossKeep;
            SaveToImage(workbook, options, "TextCrossType_CrossKeep.png");
            
            options.TextCrossType = TextCrossType.CrossOverride;
            SaveToImage(workbook, options, "TextCrossType_CrossOverride.png");
            
            options.TextCrossType = TextCrossType.StrictInCell;
            SaveToImage(workbook, options, "TextCrossType_StrictInCell.png");
        }
        
        private static void SaveToImage(Workbook workbook, ImageOrPrintOptions options, string fileName)
        {
            SheetRender sr = new SheetRender(workbook.Worksheets[0], options);
            sr.ToImage(0, fileName);
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


