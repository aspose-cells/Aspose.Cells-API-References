---
title: "Cell.SetStyle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cell. Définit le style de la cellule"
type: docs
url: /fr/net/aspose.cells/cell/setstyle/
---
## SetStyle(Style) {#setstyle}

Définit le style de la cellule.

```csharp
public void SetStyle(Style style)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| style | Style | Le style de la cellule. |

### Remarques

Si les paramètres de bordure sont modifiés, la bordure des cellules ajustées sera également mise à jour.

### Exemples

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

            // Créez un style et définissez ses propriétés
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = System.Drawing.Color.Yellow;

            // Appliquez le style à la cellule B2 (1,1 dans l'index zéro)
            cells[1, 1].SetStyle(style);

            // Enregistrez le classeur
            workbook.Save("SetStyleDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [Style](../../style/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetStyle(Style, bool) {#setstyle_2}

Applique la propriété modifiée du style à la cellule.

```csharp
public void SetStyle(Style style, bool explicitFlag)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| style | Style | Le style de la cellule. |
| explicitFlag | Boolean | True, ne remplaçant que le formatage qui est explicitement défini. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetStyleWithStyleBooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créez des styles directement
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
            
            // Appliquez des styles aux cellules avec la méthode SetStyle
            Cell cell1 = worksheet.Cells["A1"];
            cell1.PutValue("Styled Text 1");
            cell1.SetStyle(style1, true); // true to preserve existing style elements not defined in the new style
            
            Cell cell2 = worksheet.Cells["A2"];
            cell2.PutValue("Styled Text 2");
            cell2.SetStyle(style2, false); // false to overwrite all style elements
            
            // Enregistrez le classeur
            workbook.Save("SetStyleDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Style](../../style/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetStyle(Style, StyleFlag) {#setstyle_1}

Appliquer le style de la cellule en fonction des indicateurs.

```csharp
public void SetStyle(Style style, StyleFlag flag)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| style | Style | Le style de la cellule. |
| flag | StyleFlag | Le drapeau du style. |

### Exemples

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
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Créez un style et définissez ses propriétés
            Style style = workbook.CreateStyle();
            style.Font.Color = Color.Red;
            style.Name = "CustomStyle";

            // Créez un drapeau de style et définissez-le pour appliquer tout le formatage
            StyleFlag flag = new StyleFlag();
            flag.All = true;

            // Obtenez les cellules et définissez la valeur à A1
            Cells cells = sheet.Cells;
            Cell cell = cells["A1"];
            cell.PutValue("Sample Text");

            // Appliquez le style à la cellule en utilisant SetStyle
            cell.SetStyle(style, flag);

            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


