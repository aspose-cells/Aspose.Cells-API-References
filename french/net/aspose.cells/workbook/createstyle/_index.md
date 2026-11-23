---
title: "Workbook.CreateStyle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Workbook. Crée un nouveau style"
type: docs
url: /fr/net/aspose.cells/workbook/createstyle/
---
## CreateStyle() {#createstyle}

Crée un nouveau style.

```csharp
public Style CreateStyle()
```

### Valeur de retour

Renvoie un objet style.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCreateStyleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créer un nouveau style en utilisant la méthode CreateStyle
            Style newStyle = workbook.CreateStyle();
            
            // Définir les propriétés du style
            newStyle.Font.Name = "Arial";
            newStyle.Font.Size = 12;
            newStyle.Font.IsBold = true;
            newStyle.ForegroundColor = System.Drawing.Color.LightBlue;
            newStyle.Pattern = BackgroundType.Solid;
            newStyle.IsTextWrapped = true;
            
            // Créer le drapeau de style et définir les drapeaux
            StyleFlag flag = new StyleFlag();
            flag.FontName = true;
            flag.FontSize = true;
            flag.FontBold = true;
            flag.CellShading = true;
            flag.WrapText = true;
            
            // Appliquer le style à la cellule A1
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("This text has a custom style with wrapping");
            worksheet.Cells.ApplyStyle(newStyle, flag);
            
            // Ajuster automatiquement la colonne
            worksheet.AutoFitColumn(0);
            
            // Enregistrez le classeur
            workbook.Save("CreateStyleDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [Style](../../style/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateStyle(bool) {#createstyle_1}

Crée un nouveau style.

```csharp
public Style CreateStyle(bool cloneDefaultStyle)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| cloneDefaultStyle | Boolean | Indique si le style par défaut est cloné |

### Valeur de retour

Renvoie un objet style.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCreateStyleWithBooleanDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook wb = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Créer un nouveau style (false = ne pas hériter du style par défaut)
            Style style = wb.CreateStyle(false);
            style.Font.Color = System.Drawing.Color.Blue;
            style.Font.IsBold = true;
            
            // Appliquer le style à une cellule
            Cell cell = cells["A1"];
            cell.SetStyle(style);
            cell.PutValue("Styled Text");
            
            // Enregistrez le classeur
            wb.Save("CreateStyleDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [Style](../../style/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


