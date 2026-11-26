---
title: "Workbook.CreateStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Workbook. Crea un nuevo estilo"
type: docs
url: /es/net/aspose.cells/workbook/createstyle/
---
## CreateStyle() {#createstyle}

Crea un nuevo estilo.

```csharp
public Style CreateStyle()
```

### Valor de retorno

Devuelve un objeto de estilo.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCreateStyleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear un nuevo estilo usando el método CreateStyle
            Style newStyle = workbook.CreateStyle();
            
            // Establecer propiedades del estilo
            newStyle.Font.Name = "Arial";
            newStyle.Font.Size = 12;
            newStyle.Font.IsBold = true;
            newStyle.ForegroundColor = System.Drawing.Color.LightBlue;
            newStyle.Pattern = BackgroundType.Solid;
            newStyle.IsTextWrapped = true;
            
            // Crear bandera de estilo y establecer banderas
            StyleFlag flag = new StyleFlag();
            flag.FontName = true;
            flag.FontSize = true;
            flag.FontBold = true;
            flag.CellShading = true;
            flag.WrapText = true;
            
            // Aplicar el estilo a la celda A1
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("This text has a custom style with wrapping");
            worksheet.Cells.ApplyStyle(newStyle, flag);
            
            // Ajustar automáticamente la columna
            worksheet.AutoFitColumn(0);
            
            // Guarda el libro de trabajo
            workbook.Save("CreateStyleDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [Style](../../style/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateStyle(bool) {#createstyle_1}

Crea un nuevo estilo.

```csharp
public Style CreateStyle(bool cloneDefaultStyle)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cloneDefaultStyle | Booleano | Indica si clona el estilo predeterminado |

### Valor de retorno

Devuelve un objeto de estilo.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCreateStyleWithBooleanDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook wb = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Crear un nuevo estilo (false = no heredar del estilo predeterminado)
            Style style = wb.CreateStyle(false);
            style.Font.Color = System.Drawing.Color.Blue;
            style.Font.IsBold = true;
            
            // Aplicar el estilo a una celda
            Cell cell = cells["A1"];
            cell.SetStyle(style);
            cell.PutValue("Styled Text");
            
            // Guarda el libro de trabajo
            wb.Save("CreateStyleDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [Style](../../style/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


