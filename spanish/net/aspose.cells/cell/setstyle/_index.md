---
title: "Cell.SetStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cell. Establece el estilo de la celda"
type: docs
url: /es/net/aspose.cells/cell/setstyle/
---
## SetStyle(Style) {#setstyle}

Establece el estilo de la celda.

```csharp
public void SetStyle(Style style)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| estilo | Estilo | El estilo de la celda. |

### Observaciones

Si se cambian los ajustes del borde, el borde de las celdas ajustadas también se actualizará.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetStyleWithStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Crea un estilo y establece sus propiedades
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = System.Drawing.Color.Yellow;

            // Aplica el estilo a la celda B2 (1,1 en índice base cero)
            cells[1, 1].SetStyle(style);

            // Guarda el libro de trabajo
            workbook.Save("SetStyleDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [Style](../../style/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetStyle(Style, bool) {#setstyle_2}

Aplica la propiedad modificada del estilo a la celda.

```csharp
public void SetStyle(Style style, bool explicitFlag)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| estilo | Estilo | El estilo de la celda. |
| explicitFlag | Booleano | True, solo sobrescribiendo el formato que está establecido explícitamente. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetStyleWithStyleBooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea estilos directamente
            Style style1 = workbook.CreateStyle();
            style1.Name = "MyStyle1";
            style1.Font.Name = "Arial";
            style1.Font.Size = 12;
            style1.Font.IsBold = true;
            
            Style style2 = workbook.CreateStyle();
            style2.Name = "MyStyle2";
            style2.Font.Name = "Times New Roman";
            style2.Font.Size = 14;
            style2.Font.Color = System.Drawing.Color.Red;
            
            // Aplica estilos a las celdas con el método SetStyle
            Cell cell1 = worksheet.Cells["A1"];
            cell1.PutValue("Styled Text 1");
            cell1.SetStyle(style1, true); // true to preserve existing style elements not defined in the new style
            
            Cell cell2 = worksheet.Cells["A2"];
            cell2.PutValue("Styled Text 2");
            cell2.SetStyle(style2, false); // false to overwrite all style elements
            
            // Guarda el libro de trabajo
            workbook.Save("SetStyleDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Style](../../style/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetStyle(Style, StyleFlag) {#setstyle_1}

Aplicar el estilo de celda basado en banderas.

```csharp
public void SetStyle(Style style, StyleFlag flag)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| estilo | Estilo | El estilo de la celda. |
| bandera | StyleFlag | La bandera de estilo. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class CellMethodSetStyleWithStyleStyleFlagDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Crea un estilo y establece sus propiedades
            Style style = workbook.CreateStyle();
            style.Font.Color = Color.Red;
            style.Name = "CustomStyle";

            // Crea una bandera de estilo y configúrala para aplicar todo el formato
            StyleFlag flag = new StyleFlag();
            flag.All = true;

            // Obtén las celdas y establece el valor en A1
            Cells cells = sheet.Cells;
            Cell cell = cells["A1"];
            cell.PutValue("Sample Text");

            // Aplica el estilo a la celda usando SetStyle
            cell.SetStyle(style, flag);

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


