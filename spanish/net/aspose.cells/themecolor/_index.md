---
title: ThemeColor
second_title: Referencia de API de Aspose.Cells para .NET
description: Representa un color de tema.
type: docs
weight: 6000
url: /es/net/aspose.cells/themecolor/
---
## ThemeColor class

Representa un color de tema.

```csharp
public class ThemeColor
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [ThemeColor](themecolor)(ThemeColorType, double) |  |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [ColorType](../../aspose.cells/themecolor/colortype) { get; set; } | Obtiene y establece el tipo de tema. |
| [Tint](../../aspose.cells/themecolor/tint) { get; set; } | Obtiene y establece el valor de tinte. |

### Ejemplos

```csharp

[C#]

// Instanciando un objeto Workbook
Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
cells["A1"].PutValue("Hello World");
Style style = cells["A1"].GetStyle();
//Establezca el tipo de color ThemeColorType.Text2 con un 40 % de aclarado como color de fuente.
style.Font.ThemeColor = new ThemeColor(ThemeColorType.Text2, 0.4);
style.Pattern = BackgroundType.Solid;
//Establezca el tipo de color ThemeColorType.Background2 con un 75% de oscurecimiento como color de primer plano
style.ForegroundThemeColor = new ThemeColor(ThemeColorType.Background2, -0.75);
cells["A1"].SetStyle(style);
//Guardando el archivo de Excel
workbook.Save("book1.xlsx");

[Visual Basic]

'Crear una instancia de un objeto Workbook
Dim workbook As Workbook = New Workbook()
Dim cells As Cells = workbook.Worksheets(0).Cells
cells("A1").PutValue("Hello World")
'Obtener el estilo de celda
Dim style As Style = cells("A1").GetStyle()
'Establezca el tipo de color ThemeColorType.Text2 con un 40 % de aclarado como color de fuente.
Style.Font.ThemeColor = New ThemeColor(ThemeColorType.Text2, 0.4)
Style.Pattern = BackgroundType.Solid
'Establezca el tipo de color ThemeColorType.Background2 con un 75 % de oscurecimiento como color de primer plano
style.ForegroundThemeColor = New ThemeColor(ThemeColorType.Background2, -0.75)
'Establecer el estilo de celda
cells("A1").SetStyle(style)
'Guardar el archivo de Excel
Workbook.Save("book1.xlsx")
```

### Ver también

* espacio de nombres [Aspose.Cells](../../aspose.cells)
* asamblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
