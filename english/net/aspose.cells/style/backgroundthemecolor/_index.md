---
title: Style.BackgroundThemeColor
second_title: Aspose.Cells for .NET API Reference
description: Style property. Gets and sets the background theme color
type: docs
url: /net/aspose.cells/style/backgroundthemecolor/
---
## Style.BackgroundThemeColor property

Gets and sets the background theme color.

```csharp
public ThemeColor BackgroundThemeColor { get; set; }
```

### Remarks

If the background color is not a theme color, NULL will be returned.

### Examples

```csharp
// Called: ThemeColor backgroundThemeColorSrc = styleSrc.BackgroundThemeColor;
public static void Property_BackgroundThemeColor(String cellOrSheetName,Style styleSrc, Style styleDest) 
	    {   
		    // BackgroundColor
            Color bColorSrc = styleSrc.BackgroundColor; 
            Color bColorDest = styleDest.BackgroundColor;
            CompareColor.compare(cellOrSheetName + &quot; BackgroundColor &quot; ,bColorSrc,bColorDest);
        
            // ForegroundColor
            Color fColorSrc = styleSrc.ForegroundColor;
            Color fColorDest = styleDest.ForegroundColor;
            CompareColor.compare(cellOrSheetName + &quot; ForegroundColor &quot;,fColorSrc,fColorDest);
        
            // BackgroundThemeColor
            ThemeColor backgroundThemeColorSrc = styleSrc.BackgroundThemeColor;
            ThemeColor backgroundThemeColorDest = styleDest.BackgroundThemeColor;
            if(backgroundThemeColorSrc != null)
            {
                Assert.AreEqual(backgroundThemeColorSrc.ColorType, backgroundThemeColorDest.ColorType, cellOrSheetName + &quot; ColorType of BackgroundThemeColor &quot;);
	            // keep 4 digits,cut others
                Assert.AreEqual(backgroundThemeColorSrc.Tint, backgroundThemeColorDest.Tint, cellOrSheetName + &quot; Tint of BackgroundThemeColor &quot;); 
            }

            // HorizontalAlignment
            TextAlignmentType horizontalAlignmentSrc = styleSrc.HorizontalAlignment;
            TextAlignmentType horizontalAlignmentDest = styleDest.HorizontalAlignment;
            Assert.AreEqual(horizontalAlignmentSrc, horizontalAlignmentDest, cellOrSheetName + &quot; HorizontalAlignment &quot;); 

            // VerticalAlignment
            TextAlignmentType verticalAlignmentSrc = styleSrc.VerticalAlignment;
            TextAlignmentType verticalAlignmentDest = styleDest.VerticalAlignment;
            Assert.AreEqual(verticalAlignmentSrc, verticalAlignmentDest, cellOrSheetName + &quot; verticalAlignment &quot;); 
        
            // IndentLevel
            int indentLevelSrc = styleSrc.IndentLevel;
            int indentLevelDest = styleDest.IndentLevel;
            Assert.AreEqual(indentLevelSrc, indentLevelDest, cellOrSheetName + &quot; IndentLevel &quot;); 
        
            // Number
            int numberSrc = styleSrc.Number;
            int numberDest = styleDest.Number;
            Assert.AreEqual(numberSrc, numberDest, cellOrSheetName + &quot; Number &quot;); 
        
            // Pattern
            BackgroundType patternSrc = styleSrc.Pattern;
            BackgroundType patternDest = styleDest.Pattern;
            Assert.AreEqual(patternSrc, patternDest, cellOrSheetName + &quot; Pattern &quot;);  
        
            // RotationAngle;
            int rotationAngleSrc = styleSrc.RotationAngle;
            int rotationAngleDest = styleDest.RotationAngle;
            Assert.AreEqual(rotationAngleSrc, rotationAngleDest, cellOrSheetName + &quot; RotationAngle &quot;);   
        
            // TextDirection
            TextDirectionType textDirectionSrc = styleSrc.TextDirection;
            TextDirectionType textDirectionDest = styleDest.TextDirection;
            Assert.AreEqual(textDirectionSrc, textDirectionDest, cellOrSheetName + &quot; TextDirection &quot;);   

            // Font
            Aspose.Cells.Font fontSrc = styleSrc.Font; 
            Aspose.Cells.Font fontDest = styleDest.Font;
            CompareFont.compare(cellOrSheetName, fontSrc, fontDest);
        
            // CultureCustom
            String cultureCustomSrc = styleSrc.CultureCustom;
            String cultureCustomDest = styleDest.CultureCustom;
            Assert.AreEqual(cultureCustomSrc, cultureCustomDest, cellOrSheetName + &quot; CultureCustom &quot;);
        
            // Custom
            String customSrc = styleSrc.Custom;
            String customDest = styleDest.Custom;
            Assert.AreEqual(customSrc, customDest, cellOrSheetName + &quot; Custom &quot;);
        
            // Name
            String nameSrc = styleSrc.Name;
            String nameDest = styleDest.Name;
            Assert.AreEqual(nameSrc, nameDest, cellOrSheetName + &quot; Name &quot;);
        
            // ShrinkToFit
            bool shrinkToFitSrc = styleSrc.ShrinkToFit;
            bool shrinkToFitDest = styleDest.ShrinkToFit;
            Assert.AreEqual(shrinkToFitSrc, shrinkToFitDest, cellOrSheetName + &quot; ShrinkToFit &quot;);

            // TextWrapped
            bool textWrappedSrc = styleSrc.IsTextWrapped;
            bool textWrappedDest = styleDest.IsTextWrapped;
            Assert.AreEqual(textWrappedSrc, textWrappedDest, cellOrSheetName + &quot; TextWrapped &quot;);

            // TextWrapped
            bool isLockedSrc = styleSrc.IsLocked;
            bool isLockedDest = styleDest.IsLocked;
            Assert.AreEqual(isLockedSrc, isLockedDest, cellOrSheetName + &quot; Locked &quot;);

            // TextWrapped
            bool isDateTimeSrc = styleSrc.IsDateTime;
            bool isDateTimeDest = styleDest.IsDateTime;
            Assert.AreEqual(isDateTimeSrc, isDateTimeDest, cellOrSheetName + &quot; DateTime &quot;);

            // TextWrapped
            bool isFormulaHiddenSrc = styleSrc.IsFormulaHidden;
            bool isFormulaHiddenDest = styleDest.IsFormulaHidden;
            Assert.AreEqual(isFormulaHiddenSrc, isFormulaHiddenDest, cellOrSheetName + &quot; FormulaHidden &quot;);  
	    }
```

### See Also

* class [ThemeColor](../../themecolor/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


