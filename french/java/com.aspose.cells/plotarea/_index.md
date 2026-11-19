---
title: "PlotArea"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Encapsule l'objet qui représente la zone de tracé dans un graphique."
type: docs
url: /fr/java/com.aspose.cells/plotarea/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.ChartFrame](../../com.aspose.cells/chartframe)
```
public class PlotArea extends ChartFrame
```

Encapsule l'objet qui représente la zone de tracé dans un graphique.
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArea()](#getArea--) | Obtient le [getArea()](../../com.aspose.cells/chartframe\#getArea--). |
| [getAutoScaleFont()](#getAutoScaleFont--) | Vrai si le texte dans l'objet change de taille de police lorsque la taille de l'objet change. |
| [getBackground()](#getBackground--) | Obtient le mode d'affichage de l'arrière‑plan. |
| [getBackgroundMode()](#getBackgroundMode--) | Obtient le mode d'affichage de l'arrière‑plan. |
| [getBorder()](#getBorder--) | Obtient le [Line](../../com.aspose.cells/line). |
| [getChart()](#getChart--) | Obtient le graphique auquel cet objet appartient. |
| [getClass()](#getClass--) |  |
| [getDefaultHeight()](#getDefaultHeight--) | Représente la hauteur de la position par défaut en unités de 1/4000 de la zone du graphique. |
| [getDefaultHeightRatioToChart()](#getDefaultHeightRatioToChart--) | Représente la hauteur de la position par défaut en unités de la fraction de la zone du graphique. |
| [getDefaultWidth()](#getDefaultWidth--) | Représente la largeur de la position par défaut en unités de 1/4000 de la zone du graphique. |
| [getDefaultWidthRatioToChart()](#getDefaultWidthRatioToChart--) | Représente la largeur de la position par défaut en unités de fraction de la zone du graphique. |
| [getDefaultX()](#getDefaultX--) | Représente x de la position par défaut en unités de 1/4000 de la zone du graphique. |
| [getDefaultXRatioToChart()](#getDefaultXRatioToChart--) | Représente x de la position par défaut en unités de fraction de la zone du graphique. |
| [getDefaultY()](#getDefaultY--) | Représente y de la position par défaut en unités de 1/4000 de la zone du graphique. |
| [getDefaultYRatioToChart()](#getDefaultYRatioToChart--) | Représente y de la position par défaut en unités de la fraction de la zone du graphique. |
| [getFont()](#getFont--) | Obtient un objet [getFont()](../../com.aspose.cells/chartframe\#getFont--) du cadre de graphique spécifié. |
| [getHeight()](#getHeight--) | Obtient la hauteur de la boîte englobante de la zone de tracé en unités de 1/4000 de la zone du graphique. |
| [getHeightPixel()](#getHeightPixel--) | Obtient la hauteur du cadre en unités de pixels. |
| [getHeightRatioToChart()](#getHeightRatioToChart--) | Obtient la hauteur de la boîte englobante de la zone de tracé en unités du rapport de la zone du graphique. |
| [getInnerHeight()](#getInnerHeight--) | Obtient la hauteur de la zone de tracé en unités de 1/4000 de la zone du graphique. |
| [getInnerHeightRatioToChart()](#getInnerHeightRatioToChart--) | Obtient la hauteur de la zone de tracé en unités du rapport de la zone du graphique. |
| [getInnerWidth()](#getInnerWidth--) | Obtient la largeur de la zone de tracé en unités de 1/4000 de la zone du graphique. |
| [getInnerWidthRatioToChart()](#getInnerWidthRatioToChart--) | Obtient la largeur de la zone de tracé en unités du rapport de la zone du graphique. |
| [getInnerX()](#getInnerX--) | Obtient la coordonnée x du coin supérieur supérieur de la zone de tracé en unités de 1/4000 de la zone du graphique. |
| [getInnerXRatioToChart()](#getInnerXRatioToChart--) | Obtient ou obtient la coordonnée x du coin supérieur supérieur de la zone de tracé en unités du rapport de la zone du graphique. |
| [getInnerY()](#getInnerY--) | Obtient la coordonnée x du coin supérieur supérieur de la zone de tracé en unités de 1/4000 de la zone du graphique. |
| [getInnerYRatioToChart()](#getInnerYRatioToChart--) | Obtient ou obtient la coordonnée x du coin supérieur supérieur de la zone de tracé en unités du rapport de la zone du graphique. |
| [getShadow()](#getShadow--) | Vrai si le cadre possède une ombre. |
| [getShapeProperties()](#getShapeProperties--) | Obtient l'objet [getShapeProperties()](../../com.aspose.cells/chartframe\#getShapeProperties--). |
| [getTextFont()](#getTextFont--) | Obtient un objet [getFont()](../../com.aspose.cells/chartframe\#getFont--) du cadre de graphique spécifié. |
| [getTextOptions()](#getTextOptions--) | Obtient les options du texte. |
| [getWidth()](#getWidth--) | Obtient la largeur de la boîte englobante de la zone de tracé en unités de 1/4000 de la zone du graphique. |
| [getWidthPixel()](#getWidthPixel--) | Obtient la largeur du cadre en unités de Pixel. |
| [getWidthRatioToChart()](#getWidthRatioToChart--) | Obtient la largeur de la boîte englobante de la zone de tracé en unités du ratio de la zone du graphique. |
| [getX()](#getX--) | Obtient la coordonnée x du coin supérieur gauche de la boîte englobante de la zone de tracé en unités de 1/4000 de la zone du graphique. |
| [getXPixel()](#getXPixel--) | Obtient la coordonnée x du coin supérieur gauche en unités de Pixel. |
| [getXRatioToChart()](#getXRatioToChart--) | Obtient la coordonnée x du coin supérieur gauche de la boîte englobante de la zone de tracé sous forme de ratio de la zone du graphique. |
| [getY()](#getY--) | Obtient la coordonnée y du coin supérieur supérieur de la boîte englobante de la zone de tracé en unités de 1/4000 de la zone du graphique. |
| [getYPixel()](#getYPixel--) | Obtient la coordonnée y du coin supérieur gauche en unités de pixels. |
| [getYRatioToChart()](#getYRatioToChart--) | Obtient la coordonnée y du coin supérieur supérieur de la boîte englobante de la zone de tracé sous forme de ratio de la zone du graphique. |
| [hashCode()](#hashCode--) |  |
| [isAutomaticSize()](#isAutomaticSize--) | Indique si la zone de tracé est dimensionnée automatiquement. |
| [isDefaultPosBeSet()](#isDefaultPosBeSet--) | Indique si la position par défaut (DefaultX, DefaultY, DefaultWidth et DefaultHeight) est définie. |
| [isInnerMode()](#isInnerMode--) | Indique si la taille de la zone de tracé inclut les marques de graduation et les libellés des axes. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoScaleFont(boolean value)](#setAutoScaleFont-boolean-) | Vrai si le texte dans l'objet change de taille de police lorsque la taille de l'objet change. |
| [setAutomaticSize(boolean value)](#setAutomaticSize-boolean-) | Indique si la zone de tracé est dimensionnée automatiquement. |
| [setBackground(int value)](#setBackground-int-) | Définit le mode d'affichage de l'arrière-plan. |
| [setBackgroundMode(int value)](#setBackgroundMode-int-) | Définit le mode d'affichage de l'arrière-plan. |
| [setHeight(int value)](#setHeight-int-) | Définit la hauteur de la boîte englobante de la zone de tracé en unités de 1/4000 de la zone du graphique. |
| [setHeightPixel(int value)](#setHeightPixel-int-) | Définit la hauteur du cadre en unités de pixels. |
| [setHeightRatioToChart(double value)](#setHeightRatioToChart-double-) | Définit la hauteur de la boîte englobante de la zone de tracé en unités du ratio de la zone du graphique. |
| [setInnerHeight(int value)](#setInnerHeight-int-) | Définit la hauteur de la zone de tracé en unités de 1/4000 de la zone du graphique. |
| [setInnerHeightRatioToChart(double value)](#setInnerHeightRatioToChart-double-) | Définit la hauteur de la zone de tracé en unités du ratio de la zone du graphique. |
| [setInnerMode(boolean value)](#setInnerMode-boolean-) | Indique si la taille de la zone de tracé inclut les marques de graduation et les libellés des axes. |
| [setInnerWidth(int value)](#setInnerWidth-int-) | Définit la largeur de la zone de tracé en unités de 1/4000 de la zone du graphique. |
| [setInnerWidthRatioToChart(double value)](#setInnerWidthRatioToChart-double-) | Définit la largeur de la zone de tracé en unités du ratio de la zone du graphique. |
| [setInnerX(int value)](#setInnerX-int-) | Définit la coordonnée x du coin supérieur supérieur de la zone de tracé en unités de 1/4000 de la zone du graphique. |
| [setInnerXRatioToChart(double value)](#setInnerXRatioToChart-double-) | Obtient ou obtient la coordonnée x du coin supérieur supérieur de la zone de tracé en unités du rapport de la zone du graphique. |
| [setInnerY(int value)](#setInnerY-int-) | Définit la coordonnée x du coin supérieur supérieur de la zone de tracé en unités de 1/4000 de la zone du graphique. |
| [setInnerYRatioToChart(double value)](#setInnerYRatioToChart-double-) | Obtient ou obtient la coordonnée x du coin supérieur supérieur de la zone de tracé en unités du rapport de la zone du graphique. |
| [setPositionAuto()](#setPositionAuto--) | Définir la position de la zone de tracé sur automatique |
| [setShadow(boolean value)](#setShadow-boolean-) | Vrai si le cadre possède une ombre. |
| [setWidth(int value)](#setWidth-int-) | Définit la largeur de la boîte englobante de la zone de tracé en unités de 1/4000 de la zone du graphique. |
| [setWidthPixel(int value)](#setWidthPixel-int-) | Définit la largeur du cadre en unités de pixel. |
| [setWidthRatioToChart(double value)](#setWidthRatioToChart-double-) | Définit la largeur de la boîte englobante de la zone de tracé en unités du ratio de la zone du graphique. |
| [setX(int value)](#setX-int-) | Définit la coordonnée x du coin supérieur gauche de la boîte englobante de la zone de tracé en unités de 1/4000 de la zone du graphique. |
| [setXPixel(int value)](#setXPixel-int-) | Définit la coordonnée x du coin supérieur gauche en unités de pixel. |
| [setXRatioToChart(double value)](#setXRatioToChart-double-) | Définit la coordonnée x du coin supérieur gauche de la boîte englobante de la zone de tracé sous forme de ratio de la zone du graphique. |
| [setY(int value)](#setY-int-) | Définit la coordonnée y du coin supérieur supérieur de la boîte englobante de la zone de tracé en unités de 1/4000 de la zone du graphique. |
| [setYPixel(int value)](#setYPixel-int-) | Définit la coordonnée y du coin supérieur gauche en unités de pixels. |
| [setYRatioToChart(double value)](#setYRatioToChart-double-) | Définit la coordonnée y du coin supérieur supérieur de la boîte englobante de la zone de tracé sous forme de ratio de la zone du graphique. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getArea() {#getArea--}
```
public Area getArea()
```


Obtient le [getArea()](../../com.aspose.cells/chartframe\#getArea--).

**Returns:**
[Area](../../com.aspose.cells/area)
### getAutoScaleFont() {#getAutoScaleFont--}
```
public boolean getAutoScaleFont()
```


Vrai si le texte dans l'objet change de taille de police lorsque la taille de l'objet change. La valeur par défaut est Vrai.

**Returns:**
boolean
### getBackground() {#getBackground--}
```
public int getBackground()
```


Obtient le mode d'affichage de l'arrière-plan. Cette propriété n'est valable que dans Excel 2003 ou les versions antérieures.

Voir [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété ChartFrame.Area.FillFormat.FillType. Par exemple, si vous devez définir BackgroundMode sur Opaque, vous pouvez utiliser le code suivant : Area.FillFormat.FillType = FillType.Solid; Area.FillFormat.SolidFill.Color = Color.Red; Cette propriété sera supprimée 12 mois plus tard à compter de JANVIER 2012. Aspose s'excuse pour tout inconvénient que vous auriez pu rencontrer.

**Returns:**
int
### getBackgroundMode() {#getBackgroundMode--}
```
public int getBackgroundMode()
```


Obtient le mode d'affichage de l'arrière-plan. Cette propriété n'est valable que dans Excel 2003 ou les versions antérieures.

Voir [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété ChartFrame.Area.FillFormat.FillType. Par exemple, si vous devez définir BackgroundMode sur Opaque, vous pouvez utiliser le code suivant : Area.FillFormat.FillType = FillType.Solid; Area.FillFormat.SolidFill.Color = Color.Red; Cette propriété sera supprimée 12 mois plus tard à compter de février 2026. Aspose s'excuse pour tout inconvénient que vous auriez pu rencontrer.

**Returns:**
int
### getBorder() {#getBorder--}
```
public Line getBorder()
```


Obtient le [Line](../../com.aspose.cells/line).

**Returns:**
[Line](../../com.aspose.cells/line)
### getChart() {#getChart--}
```
public Chart getChart()
```


Obtient le graphique auquel cet objet appartient.

**Returns:**
[Chart](../../com.aspose.cells/chart)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDefaultHeight() {#getDefaultHeight--}
```
public int getDefaultHeight()
```


Représente la hauteur de la position par défaut en unités de 1/4000 de la zone du graphique.

**Remarks**

NOTE : Ce membre est maintenant obsolète. Veuillez plutôt utiliser la propriété ChartFrame.DefaultHeightRatioToChart. DefaultHeight = (int)(DefaultHeightRatioToChart \* 4000); Cette propriété sera supprimée 12 mois plus tard à compter de février 2025. Aspose s'excuse pour tout inconvénient que vous auriez pu rencontrer.

**Returns:**
int
### getDefaultHeightRatioToChart() {#getDefaultHeightRatioToChart--}
```
public double getDefaultHeightRatioToChart()
```


Représente la hauteur de la position par défaut en unités de la fraction de la zone du graphique.

**Returns:**
double
### getDefaultWidth() {#getDefaultWidth--}
```
public int getDefaultWidth()
```


Représente la largeur de la position par défaut en unités de 1/4000 de la zone du graphique.

**Remarks**

NOTE : Ce membre est maintenant obsolète. Veuillez plutôt utiliser la propriété ChartFrame.DefaultWidthRatioToChart. DefaultWidth = (int)(DefaultWidthRatioToChart \* 4000); Cette propriété sera supprimée 12 mois plus tard à compter de février 2025. Aspose s'excuse pour tout inconvénient que vous auriez pu rencontrer.

**Returns:**
int
### getDefaultWidthRatioToChart() {#getDefaultWidthRatioToChart--}
```
public double getDefaultWidthRatioToChart()
```


Représente la largeur de la position par défaut en unités de fraction de la zone du graphique.

**Returns:**
double
### getDefaultX() {#getDefaultX--}
```
public int getDefaultX()
```


Représente x de la position par défaut en unités de 1/4000 de la zone du graphique.

**Remarks**

NOTE : Ce membre est maintenant obsolète. Veuillez plutôt utiliser la propriété ChartFrame.DefaultXRatioToChart. DefaultX = (int)(DefaultXRatioToChart \* 4000); Cette propriété sera supprimée 12 mois plus tard à compter de février 2025. Aspose s'excuse pour tout inconvénient que vous auriez pu rencontrer.

**Returns:**
int
### getDefaultXRatioToChart() {#getDefaultXRatioToChart--}
```
public double getDefaultXRatioToChart()
```


Représente x de la position par défaut en unités de fraction de la zone du graphique.

**Returns:**
double
### getDefaultY() {#getDefaultY--}
```
public int getDefaultY()
```


Représente y de la position par défaut en unités de 1/4000 de la zone du graphique.

**Remarks**

NOTE : Ce membre est maintenant obsolète. Veuillez plutôt utiliser la propriété ChartFrame.DefaultYRatioToChart. DefaultY = (int)(DefaultYRatioToChart \* 4000); Cette propriété sera supprimée 12 mois plus tard à compter de février 2025. Aspose s'excuse pour tout inconvénient que vous auriez pu rencontrer.

**Returns:**
int
### getDefaultYRatioToChart() {#getDefaultYRatioToChart--}
```
public double getDefaultYRatioToChart()
```


Représente y de la position par défaut en unités de la fraction de la zone du graphique.

**Returns:**
double
### getFont() {#getFont--}
```
public Font getFont()
```


Obtient un objet [getFont()](../../com.aspose.cells/chartframe\#getFont--) du cadre de graphique spécifié.

**Returns:**
[Font](../../com.aspose.cells/font)
### getHeight() {#getHeight--}
```
public int getHeight()
```


Obtient la hauteur de la boîte englobante de la zone de tracé en unités de 1/4000 de la zone du graphique.

**Remarks**

NOTE : Ce membre est maintenant obsolète. Veuillez utiliser la propriété PlotArea.HeightRatioToChart à la place. Height = HeightRatioToChart \* 4000. Cette propriété sera supprimée 12 mois plus tard à compter de février 2025. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Returns:**
int
### getHeightPixel() {#getHeightPixel--}
```
public int getHeightPixel()
```


Obtient la hauteur du cadre en unités de pixels.

**Returns:**
int
### getHeightRatioToChart() {#getHeightRatioToChart--}
```
public double getHeightRatioToChart()
```


Obtient la hauteur de la boîte englobante de la zone de tracé en unités du rapport de la zone du graphique.

**Remarks**

La boîte englobante de la zone de tracé comprend la zone de tracé, les marques de graduation (étiquettes de graduation) et une petite bordure autour des marques de graduation. Si la valeur n'est pas créée par MS Excel, veuillez appeler la méthode Chart.Calculate() avant d'appeler cette méthode.

Les **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** et **HeightRatioToChart** de **PlotArea** représentent la boîte englobante de la zone de tracé qui comprend la zone de tracé, les marques de graduation (étiquettes de graduation) et une petite bordure autour des marques. Si vous souhaitez obtenir la taille réelle de la zone de tracé, vous devez appeler les propriétés **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** et **InnerHeightRatioToChart**.

Pour Excel 2007 ou version ultérieure, la valeur par défaut est zéro. Vous devez récupérer la valeur après avoir appelé Chart.Calculate().

HeightPixel = HeightRatioToChart \* chart.ChartObject.Width. Remarque : Lorsque HeightRatioToChart est défini, la propriété IsInnerMode sera automatiquement définie sur false.

**Returns:**
double
### getInnerHeight() {#getInnerHeight--}
```
public int getInnerHeight()
```


Obtient la hauteur de la zone de tracé en unités de 1/4000 de la zone du graphique.

**Remarks**

NOTE : Ce membre est maintenant obsolète. Veuillez utiliser la propriété PlotArea.InnerHeightRatioToChart à la place. InnerHeight = InnerHeightRatioToChart \* 4000 ; Cette propriété sera supprimée 12 mois plus tard, à partir de février 2025. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
int
### getInnerHeightRatioToChart() {#getInnerHeightRatioToChart--}
```
public double getInnerHeightRatioToChart()
```


Obtient la hauteur de la zone de tracé en unités du rapport de la zone du graphique.

**Remarks**

La boîte englobante de la zone de tracé comprend la zone de tracé, les marques de graduation (étiquettes de graduation) et une petite bordure autour des marques de graduation. Si la valeur n'est pas créée par MS Excel, veuillez appeler la méthode Chart.Calculate() avant d'appeler cette méthode.

Les **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** et **HeightRatioToChart** de **PlotArea** représentent la boîte englobante de la zone de tracé qui comprend la zone de tracé, les marques de graduation (étiquettes de graduation) et une petite bordure autour des marques. Si vous souhaitez obtenir la taille réelle de la zone de tracé, vous devez appeler les propriétés **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** et **InnerHeightRatioToChart**.

Pour Excel 2007 ou version ultérieure, la valeur par défaut est zéro. Vous devez récupérer la valeur après avoir appelé Chart.Calculate().

InnerHeight en pixel = InnerXRatioToChart \* chart.ChartObject.Width. Remarque : Lorsque InnerHeightRatioToChart est défini, la propriété IsInnerMode sera automatiquement définie sur True.

**Returns:**
double
### getInnerWidth() {#getInnerWidth--}
```
public int getInnerWidth()
```


Obtient la largeur de la zone de tracé en unités de 1/4000 de la zone du graphique.

**Remarks**

NOTE : Ce membre est maintenant obsolète. Veuillez utiliser la propriété PlotArea.InnerWidthRatioToChart à la place. InnerWidth = InnerWidthRatioToChart \* 4000 ; Cette propriété sera supprimée 12 mois plus tard, à partir de février 2025. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
int
### getInnerWidthRatioToChart() {#getInnerWidthRatioToChart--}
```
public double getInnerWidthRatioToChart()
```


Obtient la largeur de la zone de tracé en unités du rapport de la zone du graphique.

**Remarks**

La boîte englobante de la zone de tracé comprend la zone de tracé, les marques de graduation (étiquettes de graduation) et une petite bordure autour des marques de graduation. Si la valeur n'est pas créée par MS Excel, veuillez appeler la méthode Chart.Calculate() avant d'appeler cette méthode.

Les **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** et **HeightRatioToChart** de **PlotArea** représentent la boîte englobante de la zone de tracé qui comprend la zone de tracé, les marques de graduation (étiquettes de graduation) et une petite bordure autour des marques. Si vous souhaitez obtenir la taille réelle de la zone de tracé, vous devez appeler les propriétés **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** et **InnerHeightRatioToChart**.

Pour Excel 2007 ou version ultérieure, la valeur par défaut est zéro. Vous devez récupérer la valeur après avoir appelé Chart.Calculate().

InnerWidth en pixel = InnerXRatioToChart \* chart.ChartObject.Width. Remarque : Lorsque InnerWidthRatioToChart est défini, la propriété IsInnerMode sera automatiquement définie sur True.

**Returns:**
double
### getInnerX() {#getInnerX--}
```
public int getInnerX()
```


Obtient la coordonnée x du coin supérieur supérieur de la zone de tracé en unités de 1/4000 de la zone du graphique.

**Remarks**

NOTE : Ce membre est maintenant obsolète. Veuillez utiliser la propriété PlotArea.InnerXRatioToChart à la place. InnerX = InnerXRatioToChart \* 4000. Cette propriété sera supprimée 12 mois plus tard, à partir de février 2025. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
int
### getInnerXRatioToChart() {#getInnerXRatioToChart--}
```
public double getInnerXRatioToChart()
```


Obtient ou obtient la coordonnée x du coin supérieur supérieur de la zone de tracé en unités du rapport de la zone du graphique.

**Remarks**

La boîte englobante de la zone de tracé comprend la zone de tracé, les marques de graduation (étiquettes de graduation) et une petite bordure autour des marques de graduation. Si la valeur n'est pas créée par MS Excel, veuillez appeler la méthode Chart.Calculate() avant d'appeler cette méthode.

Les **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** et **HeightRatioToChart** de **PlotArea** représentent la boîte englobante de la zone de tracé qui comprend la zone de tracé, les marques de graduation (étiquettes de graduation) et une petite bordure autour des marques. Si vous souhaitez obtenir la taille réelle de la zone de tracé, vous devez appeler les propriétés **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** et **InnerHeightRatioToChart**.

Pour Excel 2007 ou version ultérieure, la valeur par défaut est zéro. Vous devez récupérer la valeur après avoir appelé Chart.Calculate().

InnerX en pixel = InnerXRatioToChart \* chart.ChartObject.Width. Remarque : Lorsque InnerXRatioToChart est défini, la propriété IsInnerMode sera automatiquement définie sur True.

**Returns:**
double
### getInnerY() {#getInnerY--}
```
public int getInnerY()
```


Obtient la coordonnée x du coin supérieur supérieur de la zone de tracé en unités de 1/4000 de la zone du graphique.

**Remarks**

NOTE : Ce membre est maintenant obsolète. Veuillez utiliser la propriété PlotArea.InnerYRatioToChart à la place. InnerY = InnerYRatioToChart \* 4000. Cette propriété sera supprimée 12 mois plus tard, à partir de février 2025. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
int
### getInnerYRatioToChart() {#getInnerYRatioToChart--}
```
public double getInnerYRatioToChart()
```


Obtient ou obtient la coordonnée x du coin supérieur supérieur de la zone de tracé en unités du rapport de la zone du graphique.

**Remarks**

La boîte englobante de la zone de tracé comprend la zone de tracé, les marques de graduation (étiquettes de graduation) et une petite bordure autour des marques de graduation. Si la valeur n'est pas créée par MS Excel, veuillez appeler la méthode Chart.Calculate() avant d'appeler cette méthode.

Les **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** et **HeightRatioToChart** de **PlotArea** représentent la boîte englobante de la zone de tracé qui comprend la zone de tracé, les marques de graduation (étiquettes de graduation) et une petite bordure autour des marques. Si vous souhaitez obtenir la taille réelle de la zone de tracé, vous devez appeler les propriétés **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** et **InnerHeightRatioToChart**.

Pour Excel 2007 ou version ultérieure, la valeur par défaut est zéro. Vous devez récupérer la valeur après avoir appelé Chart.Calculate().

InnerY en pixel = InnerYRatioToChart \* chart.ChartObject.Width. Remarque : Lorsque InnerYRatioToChart est défini, la propriété IsInnerMode sera automatiquement définie sur True.

**Returns:**
double
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


Vrai si le cadre possède une ombre.

**Remarks**

Uniquement pour les graphiques dans les fichiers xls.

**Returns:**
boolean
### getShapeProperties() {#getShapeProperties--}
```
public ShapePropertyCollection getShapeProperties()
```


Obtient l'objet [getShapeProperties()](../../com.aspose.cells/chartframe\#getShapeProperties--).

**Returns:**
[ShapePropertyCollection](../../com.aspose.cells/shapepropertycollection)
### getTextFont() {#getTextFont--}
```
public Font getTextFont()
```


Obtient un objet [getFont()](../../com.aspose.cells/chartframe\#getFont--) du cadre de graphique spécifié.

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété ChartFrame.Font. Cette propriété sera supprimée 12 mois plus tard à compter de janvier 2012. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Returns:**
[Font](../../com.aspose.cells/font)
### getTextOptions() {#getTextOptions--}
```
public TextOptions getTextOptions()
```


Obtient les options du texte.

**Returns:**
[TextOptions](../../com.aspose.cells/textoptions)
### getWidth() {#getWidth--}
```
public int getWidth()
```


Obtient la largeur de la boîte englobante de la zone de tracé en unités de 1/4000 de la zone du graphique.

**Remarks**

NOTE : Ce membre est maintenant obsolète. Veuillez utiliser la propriété PlotArea.WidthRatioToChart à la place. Width = WidthRatioToChart \* 4000. Cette propriété sera supprimée 12 mois plus tard, à partir de février 2025. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
int
### getWidthPixel() {#getWidthPixel--}
```
public int getWidthPixel()
```


Obtient la largeur du cadre en unités de Pixel.

**Returns:**
int
### getWidthRatioToChart() {#getWidthRatioToChart--}
```
public double getWidthRatioToChart()
```


Obtient la largeur de la boîte englobante de la zone de tracé en unités du ratio de la zone du graphique.

**Remarks**

La boîte englobante de la zone de tracé comprend la zone de tracé, les marques de graduation (étiquettes de graduation) et une petite bordure autour des marques de graduation. Si la valeur n'est pas créée par MS Excel, veuillez appeler la méthode Chart.Calculate() avant d'appeler cette méthode.

Les **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** et **HeightRatioToChart** de **PlotArea** représentent la boîte englobante de la zone de tracé qui comprend la zone de tracé, les marques de graduation (étiquettes de graduation) et une petite bordure autour des marques. Si vous souhaitez obtenir la taille réelle de la zone de tracé, vous devez appeler les propriétés **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** et **InnerHeightRatioToChart**.

Pour Excel 2007 ou version ultérieure, la valeur par défaut est zéro. Vous devez récupérer la valeur après avoir appelé Chart.Calculate().

WidthPixel = WidthRatioToChart \* chart.ChartObject.Width. Remarque : Lorsque WidthRatioToChart est défini, la propriété IsInnerMode sera automatiquement définie sur false.

**Returns:**
double
### getX() {#getX--}
```
public int getX()
```


Obtient la coordonnée x du coin supérieur gauche de la boîte englobante de la zone de tracé en unités de 1/4000 de la zone du graphique.

**Remarks**

NOTE : Ce membre est maintenant obsolète. Veuillez utiliser la propriété PlotArea.XRatioToChart à la place. X = XRatioToChart \* 4000. Cette propriété sera supprimée 12 mois plus tard, à partir de février 2025. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
int
### getXPixel() {#getXPixel--}
```
public int getXPixel()
```


Obtient la coordonnée x du coin supérieur gauche en unités de Pixel.

**Returns:**
int
### getXRatioToChart() {#getXRatioToChart--}
```
public double getXRatioToChart()
```


Obtient la coordonnée x du coin supérieur gauche de la boîte englobante de la zone de tracé sous forme de ratio de la zone du graphique.

**Remarks**

La boîte englobante de la zone de tracé comprend la zone de tracé, les marques de graduation (étiquettes de graduation) et une petite bordure autour des marques de graduation. Si la valeur n'est pas créée par MS Excel, veuillez appeler la méthode Chart.Calculate() avant d'appeler cette méthode.

Les **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** et **HeightRatioToChart** de **PlotArea** représentent la boîte englobante de la zone de tracé qui comprend la zone de tracé, les marques de graduation (étiquettes de graduation) et une petite bordure autour des marques. Si vous souhaitez obtenir la taille réelle de la zone de tracé, vous devez appeler les propriétés **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** et **InnerHeightRatioToChart**.

Pour Excel 2007 ou version ultérieure, la valeur par défaut est zéro. Vous devez récupérer la valeur après avoir appelé Chart.Calculate().

XPixel = XRatioToChart \* chart.ChartObject.Width. Remarque : Lorsque XRatioToChart est défini, la propriété IsInnerMode sera automatiquement définie sur false.

**Returns:**
double
### getY() {#getY--}
```
public int getY()
```


Obtient la coordonnée y du coin supérieur supérieur de la boîte englobante de la zone de tracé en unités de 1/4000 de la zone du graphique.

**Remarks**

NOTE : Ce membre est maintenant obsolète. Veuillez utiliser la propriété PlotArea.YRatioToChart à la place. Y = YRatioToChart \* 4000. Cette propriété sera supprimée 12 mois plus tard, à partir de février 2025. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Returns:**
int
### getYPixel() {#getYPixel--}
```
public int getYPixel()
```


Obtient la coordonnée y du coin supérieur gauche en unités de pixels.

**Returns:**
int
### getYRatioToChart() {#getYRatioToChart--}
```
public double getYRatioToChart()
```


Obtient la coordonnée y du coin supérieur supérieur de la boîte englobante de la zone de tracé sous forme de ratio de la zone du graphique.

**Remarks**

La boîte englobante de la zone de tracé comprend la zone de tracé, les marques de graduation (étiquettes de graduation) et une petite bordure autour des marques de graduation. Si la valeur n'est pas créée par MS Excel, veuillez appeler la méthode Chart.Calculate() avant d'appeler cette méthode.

Les **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** et **HeightRatioToChart** de **PlotArea** représentent la boîte englobante de la zone de tracé qui comprend la zone de tracé, les marques de graduation (étiquettes de graduation) et une petite bordure autour des marques. Si vous souhaitez obtenir la taille réelle de la zone de tracé, vous devez appeler les propriétés **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** et **InnerHeightRatioToChart**.

Pour Excel 2007 ou version ultérieure, la valeur par défaut est zéro. Vous devez récupérer la valeur après avoir appelé Chart.Calculate().

YPixel = YRatioToChart \* chart.ChartObject.Width. Remarque : Lorsque YRatioToChart est défini, la propriété IsInnerMode sera automatiquement définie sur false.

**Returns:**
double
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutomaticSize() {#isAutomaticSize--}
```
public boolean isAutomaticSize()
```


Indique si la zone de tracé est dimensionnée automatiquement.

**Remarks**

NOTE : Lorsque IsAutomaticSize est défini sur True, les valeurs que vous avez définies manuellement pour Width et Height seront désactivées.

**Returns:**
boolean
### isDefaultPosBeSet() {#isDefaultPosBeSet--}
```
public boolean isDefaultPosBeSet()
```


Indique si la position par défaut (DefaultX, DefaultY, DefaultWidth et DefaultHeight) est définie.

**Returns:**
boolean
### isInnerMode() {#isInnerMode--}
```
public boolean isInnerMode()
```


Indique si la taille de la zone de tracé inclut les marques de graduation et les étiquettes d'axe. False spécifie que la taille doit déterminer la taille de la zone de tracé, les marques de graduation et les étiquettes d'axe.

**Remarks**

Uniquement pour les fichiers Xlsx.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAutoScaleFont(boolean value) {#setAutoScaleFont-boolean-}
```
public void setAutoScaleFont(boolean value)
```


Vrai si le texte dans l'objet change de taille de police lorsque la taille de l'objet change. La valeur par défaut est Vrai.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setAutomaticSize(boolean value) {#setAutomaticSize-boolean-}
```
public void setAutomaticSize(boolean value)
```


Indique si la zone de tracé est dimensionnée automatiquement.

**Remarks**

NOTE : Lorsque IsAutomaticSize est défini sur True, les valeurs que vous avez définies manuellement pour Width et Height seront désactivées.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setBackground(int value) {#setBackground-int-}
```
public void setBackground(int value)
```


Définit le mode d'affichage de l'arrière-plan. Cette propriété n'est valable que dans Excel 2003 ou les versions antérieures.

Voir [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété ChartFrame.Area.FillFormat.FillType. Par exemple, si vous devez définir BackgroundMode sur Opaque, vous pouvez utiliser le code suivant : Area.FillFormat.FillType = FillType.Solid; Area.FillFormat.SolidFill.Color = Color.Red; Cette propriété sera supprimée 12 mois plus tard à compter de JANVIER 2012. Aspose s'excuse pour tout inconvénient que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setBackgroundMode(int value) {#setBackgroundMode-int-}
```
public void setBackgroundMode(int value)
```


Définit le mode d'affichage de l'arrière-plan. Cette propriété n'est valable que dans Excel 2003 ou les versions antérieures.

Voir [BackgroundMode](../../com.aspose.cells/backgroundmode).

**Remarks**

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété ChartFrame.Area.FillFormat.FillType. Par exemple, si vous devez définir BackgroundMode sur Opaque, vous pouvez utiliser le code suivant : Area.FillFormat.FillType = FillType.Solid; Area.FillFormat.SolidFill.Color = Color.Red; Cette propriété sera supprimée 12 mois plus tard à compter de février 2026. Aspose s'excuse pour tout inconvénient que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setHeight(int value) {#setHeight-int-}
```
public void setHeight(int value)
```


Définit la hauteur de la boîte englobante de la zone de tracé en unités de 1/4000 de la zone du graphique.

**Remarks**

NOTE : Ce membre est maintenant obsolète. Veuillez utiliser la propriété PlotArea.HeightRatioToChart à la place. Height = HeightRatioToChart \* 4000. Cette propriété sera supprimée 12 mois plus tard à compter de février 2025. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setHeightPixel(int value) {#setHeightPixel-int-}
```
public void setHeightPixel(int value)
```


Définit la hauteur du cadre en unités de pixels.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setHeightRatioToChart(double value) {#setHeightRatioToChart-double-}
```
public void setHeightRatioToChart(double value)
```


Définit la hauteur de la boîte englobante de la zone de tracé en unités du ratio de la zone du graphique.

**Remarks**

La boîte englobante de la zone de tracé comprend la zone de tracé, les marques de graduation (étiquettes de graduation) et une petite bordure autour des marques de graduation. Si la valeur n'est pas créée par MS Excel, veuillez appeler la méthode Chart.Calculate() avant d'appeler cette méthode.

Les **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** et **HeightRatioToChart** de **PlotArea** représentent la boîte englobante de la zone de tracé qui comprend la zone de tracé, les marques de graduation (étiquettes de graduation) et une petite bordure autour des marques. Si vous souhaitez obtenir la taille réelle de la zone de tracé, vous devez appeler les propriétés **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** et **InnerHeightRatioToChart**.

Pour Excel 2007 ou version ultérieure, la valeur par défaut est zéro. Vous devez récupérer la valeur après avoir appelé Chart.Calculate().

HeightPixel = HeightRatioToChart \* chart.ChartObject.Width. Remarque : Lorsque HeightRatioToChart est défini, la propriété IsInnerMode sera automatiquement définie sur false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setInnerHeight(int value) {#setInnerHeight-int-}
```
public void setInnerHeight(int value)
```


Définit la hauteur de la zone de tracé en unités de 1/4000 de la zone du graphique.

**Remarks**

NOTE : Ce membre est maintenant obsolète. Veuillez utiliser la propriété PlotArea.InnerHeightRatioToChart à la place. InnerHeight = InnerHeightRatioToChart \* 4000 ; Cette propriété sera supprimée 12 mois plus tard, à partir de février 2025. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setInnerHeightRatioToChart(double value) {#setInnerHeightRatioToChart-double-}
```
public void setInnerHeightRatioToChart(double value)
```


Définit la hauteur de la zone de tracé en unités du ratio de la zone du graphique.

**Remarks**

La boîte englobante de la zone de tracé comprend la zone de tracé, les marques de graduation (étiquettes de graduation) et une petite bordure autour des marques de graduation. Si la valeur n'est pas créée par MS Excel, veuillez appeler la méthode Chart.Calculate() avant d'appeler cette méthode.

Les **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** et **HeightRatioToChart** de **PlotArea** représentent la boîte englobante de la zone de tracé qui comprend la zone de tracé, les marques de graduation (étiquettes de graduation) et une petite bordure autour des marques. Si vous souhaitez obtenir la taille réelle de la zone de tracé, vous devez appeler les propriétés **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** et **InnerHeightRatioToChart**.

Pour Excel 2007 ou version ultérieure, la valeur par défaut est zéro. Vous devez récupérer la valeur après avoir appelé Chart.Calculate().

InnerHeight en pixel = InnerXRatioToChart \* chart.ChartObject.Width. Remarque : Lorsque InnerHeightRatioToChart est défini, la propriété IsInnerMode sera automatiquement définie sur True.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setInnerMode(boolean value) {#setInnerMode-boolean-}
```
public void setInnerMode(boolean value)
```


Indique si la taille de la zone de tracé inclut les marques de graduation et les étiquettes d'axe. False spécifie que la taille doit déterminer la taille de la zone de tracé, les marques de graduation et les étiquettes d'axe.

**Remarks**

Uniquement pour les fichiers Xlsx.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setInnerWidth(int value) {#setInnerWidth-int-}
```
public void setInnerWidth(int value)
```


Définit la largeur de la zone de tracé en unités de 1/4000 de la zone du graphique.

**Remarks**

NOTE : Ce membre est maintenant obsolète. Veuillez utiliser la propriété PlotArea.InnerWidthRatioToChart à la place. InnerWidth = InnerWidthRatioToChart \* 4000 ; Cette propriété sera supprimée 12 mois plus tard, à partir de février 2025. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setInnerWidthRatioToChart(double value) {#setInnerWidthRatioToChart-double-}
```
public void setInnerWidthRatioToChart(double value)
```


Définit la largeur de la zone de tracé en unités du ratio de la zone du graphique.

**Remarks**

La boîte englobante de la zone de tracé comprend la zone de tracé, les marques de graduation (étiquettes de graduation) et une petite bordure autour des marques de graduation. Si la valeur n'est pas créée par MS Excel, veuillez appeler la méthode Chart.Calculate() avant d'appeler cette méthode.

Les **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** et **HeightRatioToChart** de **PlotArea** représentent la boîte englobante de la zone de tracé qui comprend la zone de tracé, les marques de graduation (étiquettes de graduation) et une petite bordure autour des marques. Si vous souhaitez obtenir la taille réelle de la zone de tracé, vous devez appeler les propriétés **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** et **InnerHeightRatioToChart**.

Pour Excel 2007 ou version ultérieure, la valeur par défaut est zéro. Vous devez récupérer la valeur après avoir appelé Chart.Calculate().

InnerWidth en pixel = InnerXRatioToChart \* chart.ChartObject.Width. Remarque : Lorsque InnerWidthRatioToChart est défini, la propriété IsInnerMode sera automatiquement définie sur True.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setInnerX(int value) {#setInnerX-int-}
```
public void setInnerX(int value)
```


Définit la coordonnée x du coin supérieur supérieur de la zone de tracé en unités de 1/4000 de la zone du graphique.

**Remarks**

NOTE : Ce membre est maintenant obsolète. Veuillez utiliser la propriété PlotArea.InnerXRatioToChart à la place. InnerX = InnerXRatioToChart \* 4000. Cette propriété sera supprimée 12 mois plus tard, à partir de février 2025. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setInnerXRatioToChart(double value) {#setInnerXRatioToChart-double-}
```
public void setInnerXRatioToChart(double value)
```


Obtient ou obtient la coordonnée x du coin supérieur supérieur de la zone de tracé en unités du rapport de la zone du graphique.

**Remarks**

La boîte englobante de la zone de tracé comprend la zone de tracé, les marques de graduation (étiquettes de graduation) et une petite bordure autour des marques de graduation. Si la valeur n'est pas créée par MS Excel, veuillez appeler la méthode Chart.Calculate() avant d'appeler cette méthode.

Les **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** et **HeightRatioToChart** de **PlotArea** représentent la boîte englobante de la zone de tracé qui comprend la zone de tracé, les marques de graduation (étiquettes de graduation) et une petite bordure autour des marques. Si vous souhaitez obtenir la taille réelle de la zone de tracé, vous devez appeler les propriétés **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** et **InnerHeightRatioToChart**.

Pour Excel 2007 ou version ultérieure, la valeur par défaut est zéro. Vous devez récupérer la valeur après avoir appelé Chart.Calculate().

InnerX en pixel = InnerXRatioToChart \* chart.ChartObject.Width. Remarque : Lorsque InnerXRatioToChart est défini, la propriété IsInnerMode sera automatiquement définie sur True.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setInnerY(int value) {#setInnerY-int-}
```
public void setInnerY(int value)
```


Définit la coordonnée x du coin supérieur supérieur de la zone de tracé en unités de 1/4000 de la zone du graphique.

**Remarks**

NOTE : Ce membre est maintenant obsolète. Veuillez utiliser la propriété PlotArea.InnerYRatioToChart à la place. InnerY = InnerYRatioToChart \* 4000. Cette propriété sera supprimée 12 mois plus tard, à partir de février 2025. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setInnerYRatioToChart(double value) {#setInnerYRatioToChart-double-}
```
public void setInnerYRatioToChart(double value)
```


Obtient ou obtient la coordonnée x du coin supérieur supérieur de la zone de tracé en unités du rapport de la zone du graphique.

**Remarks**

La boîte englobante de la zone de tracé comprend la zone de tracé, les marques de graduation (étiquettes de graduation) et une petite bordure autour des marques de graduation. Si la valeur n'est pas créée par MS Excel, veuillez appeler la méthode Chart.Calculate() avant d'appeler cette méthode.

Les **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** et **HeightRatioToChart** de **PlotArea** représentent la boîte englobante de la zone de tracé qui comprend la zone de tracé, les marques de graduation (étiquettes de graduation) et une petite bordure autour des marques. Si vous souhaitez obtenir la taille réelle de la zone de tracé, vous devez appeler les propriétés **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** et **InnerHeightRatioToChart**.

Pour Excel 2007 ou version ultérieure, la valeur par défaut est zéro. Vous devez récupérer la valeur après avoir appelé Chart.Calculate().

InnerY en pixel = InnerYRatioToChart \* chart.ChartObject.Width. Remarque : Lorsque InnerYRatioToChart est défini, la propriété IsInnerMode sera automatiquement définie sur True.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setPositionAuto() {#setPositionAuto--}
```
public void setPositionAuto()
```


Définir la position de la zone de tracé sur automatique

### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```


Vrai si le cadre possède une ombre.

**Remarks**

Uniquement pour les graphiques dans les fichiers xls.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setWidth(int value) {#setWidth-int-}
```
public void setWidth(int value)
```


Définit la largeur de la boîte englobante de la zone de tracé en unités de 1/4000 de la zone du graphique.

**Remarks**

NOTE : Ce membre est maintenant obsolète. Veuillez utiliser la propriété PlotArea.WidthRatioToChart à la place. Width = WidthRatioToChart \* 4000. Cette propriété sera supprimée 12 mois plus tard, à partir de février 2025. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setWidthPixel(int value) {#setWidthPixel-int-}
```
public void setWidthPixel(int value)
```


Définit la largeur du cadre en unités de pixel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setWidthRatioToChart(double value) {#setWidthRatioToChart-double-}
```
public void setWidthRatioToChart(double value)
```


Définit la largeur de la boîte englobante de la zone de tracé en unités du ratio de la zone du graphique.

**Remarks**

La boîte englobante de la zone de tracé comprend la zone de tracé, les marques de graduation (étiquettes de graduation) et une petite bordure autour des marques de graduation. Si la valeur n'est pas créée par MS Excel, veuillez appeler la méthode Chart.Calculate() avant d'appeler cette méthode.

Les **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** et **HeightRatioToChart** de **PlotArea** représentent la boîte englobante de la zone de tracé qui comprend la zone de tracé, les marques de graduation (étiquettes de graduation) et une petite bordure autour des marques. Si vous souhaitez obtenir la taille réelle de la zone de tracé, vous devez appeler les propriétés **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** et **InnerHeightRatioToChart**.

Pour Excel 2007 ou version ultérieure, la valeur par défaut est zéro. Vous devez récupérer la valeur après avoir appelé Chart.Calculate().

WidthPixel = WidthRatioToChart \* chart.ChartObject.Width. Remarque : Lorsque WidthRatioToChart est défini, la propriété IsInnerMode sera automatiquement définie sur false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setX(int value) {#setX-int-}
```
public void setX(int value)
```


Définit la coordonnée x du coin supérieur gauche de la boîte englobante de la zone de tracé en unités de 1/4000 de la zone du graphique.

**Remarks**

NOTE : Ce membre est maintenant obsolète. Veuillez utiliser la propriété PlotArea.XRatioToChart à la place. X = XRatioToChart \* 4000. Cette propriété sera supprimée 12 mois plus tard, à partir de février 2025. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setXPixel(int value) {#setXPixel-int-}
```
public void setXPixel(int value)
```


Définit la coordonnée x du coin supérieur gauche en unités de pixel.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setXRatioToChart(double value) {#setXRatioToChart-double-}
```
public void setXRatioToChart(double value)
```


Définit la coordonnée x du coin supérieur gauche de la boîte englobante de la zone de tracé sous forme de ratio de la zone du graphique.

**Remarks**

La boîte englobante de la zone de tracé comprend la zone de tracé, les marques de graduation (étiquettes de graduation) et une petite bordure autour des marques de graduation. Si la valeur n'est pas créée par MS Excel, veuillez appeler la méthode Chart.Calculate() avant d'appeler cette méthode.

Les **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** et **HeightRatioToChart** de **PlotArea** représentent la boîte englobante de la zone de tracé qui comprend la zone de tracé, les marques de graduation (étiquettes de graduation) et une petite bordure autour des marques. Si vous souhaitez obtenir la taille réelle de la zone de tracé, vous devez appeler les propriétés **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** et **InnerHeightRatioToChart**.

Pour Excel 2007 ou version ultérieure, la valeur par défaut est zéro. Vous devez récupérer la valeur après avoir appelé Chart.Calculate().

XPixel = XRatioToChart \* chart.ChartObject.Width. Remarque : Lorsque XRatioToChart est défini, la propriété IsInnerMode sera automatiquement définie sur false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### setY(int value) {#setY-int-}
```
public void setY(int value)
```


Définit la coordonnée y du coin supérieur supérieur de la boîte englobante de la zone de tracé en unités de 1/4000 de la zone du graphique.

**Remarks**

NOTE : Ce membre est maintenant obsolète. Veuillez utiliser la propriété PlotArea.YRatioToChart à la place. Y = YRatioToChart \* 4000. Cette propriété sera supprimée 12 mois plus tard, à partir de février 2025. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setYPixel(int value) {#setYPixel-int-}
```
public void setYPixel(int value)
```


Définit la coordonnée y du coin supérieur gauche en unités de pixels.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setYRatioToChart(double value) {#setYRatioToChart-double-}
```
public void setYRatioToChart(double value)
```


Définit la coordonnée y du coin supérieur supérieur de la boîte englobante de la zone de tracé sous forme de ratio de la zone du graphique.

**Remarks**

La boîte englobante de la zone de tracé comprend la zone de tracé, les marques de graduation (étiquettes de graduation) et une petite bordure autour des marques de graduation. Si la valeur n'est pas créée par MS Excel, veuillez appeler la méthode Chart.Calculate() avant d'appeler cette méthode.

Les **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** et **HeightRatioToChart** de **PlotArea** représentent la boîte englobante de la zone de tracé qui comprend la zone de tracé, les marques de graduation (étiquettes de graduation) et une petite bordure autour des marques. Si vous souhaitez obtenir la taille réelle de la zone de tracé, vous devez appeler les propriétés **InnerXRatioToChart**, **InnerYRatioToChart**, **InnerWidthRatioToChart** et **InnerHeightRatioToChart**.

Pour Excel 2007 ou version ultérieure, la valeur par défaut est zéro. Vous devez récupérer la valeur après avoir appelé Chart.Calculate().

YPixel = YRatioToChart \* chart.ChartObject.Width. Remarque : Lorsque YRatioToChart est défini, la propriété IsInnerMode sera automatiquement définie sur false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

