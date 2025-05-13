---
title: ThemeColor.Tint
second_title: Aspose.Cells for .NET API Reference
description: ThemeColor property. Gets and sets the tint value
type: docs
url: /net/aspose.cells/themecolor/tint/
---
## ThemeColor.Tint property

Gets and sets the tint value.

```csharp
public double Tint { get; set; }
```

### Remarks

The tint value is stored as a double from -1.0 .. 1.0, where -1.0 means 100% darken and 1.0 means 100% lighten. Also, 0.0 means no change.

### Examples

```csharp
// Called: Assert.AreEqual(backgroundThemeColorSrc.Tint, backgroundThemeColorDest.Tint, cellOrSheetName + " Tint of BackgroundThemeColor ");
public static void ThemeColor_Property_Tint(String cellOrSheetName,Style styleSrc, Style styleDest) 
	    {   
		    // BackgroundColor
            Color bColorSrc = styleSrc.BackgroundColor; 
            Color bColorDest = styleDest.BackgroundColor;
            CompareColor.compare(cellOrSheetName + " BackgroundColor " ,bColorSrc,bColorDest);
        
            // ForegroundColor
            Color fColorSrc = styleSrc.ForegroundColor;
            Color fColorDest = styleDest.ForegroundColor;
            CompareColor.compare(cellOrSheetName + " ForegroundColor ",fColorSrc,fColorDest);
        
            // BackgroundThemeColor
            ThemeColor backgroundThemeColorSrc = styleSrc.BackgroundThemeColor;
            ThemeColor backgroundThemeColorDest = styleDest.BackgroundThemeColor;
            if(backgroundThemeColorSrc != null)
            {
                Assert.AreEqual(backgroundThemeColorSrc.ColorType, backgroundThemeColorDest.ColorType, cellOrSheetName + " ColorType of BackgroundThemeColor ");
	            // keep 4 digits,cut others
                Assert.AreEqual(backgroundThemeColorSrc.Tint, backgroundThemeColorDest.Tint, cellOrSheetName + " Tint of BackgroundThemeColor "); 
            }

            // HorizontalAlignment
            TextAlignmentType horizontalAlignmentSrc = styleSrc.HorizontalAlignment;
            TextAlignmentType horizontalAlignmentDest = styleDest.HorizontalAlignment;
            Assert.AreEqual(horizontalAlignmentSrc, horizontalAlignmentDest, cellOrSheetName + " HorizontalAlignment "); 

            // VerticalAlignment
            TextAlignmentType verticalAlignmentSrc = styleSrc.VerticalAlignment;
            TextAlignmentType verticalAlignmentDest = styleDest.VerticalAlignment;
            Assert.AreEqual(verticalAlignmentSrc, verticalAlignmentDest, cellOrSheetName + " verticalAlignment "); 
        
            // IndentLevel
            int indentLevelSrc = styleSrc.IndentLevel;
            int indentLevelDest = styleDest.IndentLevel;
            Assert.AreEqual(indentLevelSrc, indentLevelDest, cellOrSheetName + " IndentLevel "); 
        
            // Number
            int numberSrc = styleSrc.Number;
            int numberDest = styleDest.Number;
            Assert.AreEqual(numberSrc, numberDest, cellOrSheetName + " Number "); 
        
            // Pattern
            BackgroundType patternSrc = styleSrc.Pattern;
            BackgroundType patternDest = styleDest.Pattern;
            Assert.AreEqual(patternSrc, patternDest, cellOrSheetName + " Pattern ");  
        
            // RotationAngle;
            int rotationAngleSrc = styleSrc.RotationAngle;
            int rotationAngleDest = styleDest.RotationAngle;
            Assert.AreEqual(rotationAngleSrc, rotationAngleDest, cellOrSheetName + " RotationAngle ");   
        
            // TextDirection
            TextDirectionType textDirectionSrc = styleSrc.TextDirection;
            TextDirectionType textDirectionDest = styleDest.TextDirection;
            Assert.AreEqual(textDirectionSrc, textDirectionDest, cellOrSheetName + " TextDirection ");   

            // Font
            Aspose.Cells.Font fontSrc = styleSrc.Font; 
            Aspose.Cells.Font fontDest = styleDest.Font;
            CompareFont.compare(cellOrSheetName, fontSrc, fontDest);
        
            // CultureCustom
            String cultureCustomSrc = styleSrc.CultureCustom;
            String cultureCustomDest = styleDest.CultureCustom;
            Assert.AreEqual(cultureCustomSrc, cultureCustomDest, cellOrSheetName + " CultureCustom ");
        
            // Custom
            String customSrc = styleSrc.Custom;
            String customDest = styleDest.Custom;
            Assert.AreEqual(customSrc, customDest, cellOrSheetName + " Custom ");
        
            // Name
            String nameSrc = styleSrc.Name;
            String nameDest = styleDest.Name;
            Assert.AreEqual(nameSrc, nameDest, cellOrSheetName + " Name ");
        
            // ShrinkToFit
            bool shrinkToFitSrc = styleSrc.ShrinkToFit;
            bool shrinkToFitDest = styleDest.ShrinkToFit;
            Assert.AreEqual(shrinkToFitSrc, shrinkToFitDest, cellOrSheetName + " ShrinkToFit ");

            // TextWrapped
            bool textWrappedSrc = styleSrc.IsTextWrapped;
            bool textWrappedDest = styleDest.IsTextWrapped;
            Assert.AreEqual(textWrappedSrc, textWrappedDest, cellOrSheetName + " TextWrapped ");

            // TextWrapped
            bool isLockedSrc = styleSrc.IsLocked;
            bool isLockedDest = styleDest.IsLocked;
            Assert.AreEqual(isLockedSrc, isLockedDest, cellOrSheetName + " Locked ");

            // TextWrapped
            bool isDateTimeSrc = styleSrc.IsDateTime;
            bool isDateTimeDest = styleDest.IsDateTime;
            Assert.AreEqual(isDateTimeSrc, isDateTimeDest, cellOrSheetName + " DateTime ");

            // TextWrapped
            bool isFormulaHiddenSrc = styleSrc.IsFormulaHidden;
            bool isFormulaHiddenDest = styleDest.IsFormulaHidden;
            Assert.AreEqual(isFormulaHiddenSrc, isFormulaHiddenDest, cellOrSheetName + " FormulaHidden ");  
	    }
```

### See Also

* class [ThemeColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


