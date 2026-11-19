---
title: "GridTableItemStyle"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Hérité de System.Web.UI.WebControls.TableItemStyle."
type: docs
url: /fr/java/com.aspose.gridweb/gridtableitemstyle/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.WebStyle](../../com.aspose.gridweb/webstyle), [com.aspose.gridweb.WebTableItemStyle](../../com.aspose.gridweb/webtableitemstyle)
```
public class GridTableItemStyle extends WebTableItemStyle
```

Hérité de System.Web.UI.WebControls.TableItemStyle. Encapsule les styles d'une WebCell.

**Example**

```
         GridWeb GridWeb1 = new GridWeb();
         GridWorksheetCollection sheets = GridWeb1.getWorkSheets();
 
         GridWorksheet sheet = sheets.add("demo1");
 
         sheet.getCells().get(0,0).putValue("Demo Text");
         GridTableItemStyle style = sheet.getCells().get(0, 0).getStyle();
 
         style.getFont().setSize(FontUnit.Point(72));
         style.setWrap(false);
 
         style.setBackColor(Color.getGray());
         	style.setBorderStyle(com.aspose.gridweb.BorderStyle.Solid);
         style.setBorderWidth(Unit.Pixel(1));
         style.setBorderColor(Color.getSilver());
         style.getRightBorderStyle().setBorderColor(Color.getBlack());
         	style.getRightBorderStyle().setBorderStyle(com.aspose.gridweb.BorderStyle.Solid);
         	style.getRightBorderStyle().setBorderWidth(Unit.Pixel(1));
         style.getBottomBorderStyle().setBorderColor(Color.getBlack());
         style.getBottomBorderStyle().setBorderStyle(com.aspose.gridweb.BorderStyle.Solid);
         style.getBottomBorderStyle().setBorderWidth(Unit.Pixel(1));
         sheet.getCells().get(0, 0).setStyle(style);
```
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [GridTableItemStyle()](#GridTableItemStyle--) | Constructeur par défaut. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [copyFrom(WebStyle s)](#copyFrom-com.aspose.gridweb.WebStyle-) | Copie à partir d'un autre objet de style. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackColor()](#getBackColor--) | Obtient la BackColor dans le style |
| [getBackImageAttributes()](#getBackImageAttributes--) | Attributs de l'image d'arrière-plan. |
| [getBackImageUrl()](#getBackImageUrl--) | URL de l'image d'arrière-plan. |
| [getBorderColor()](#getBorderColor--) | Obtient la BorderColor dans le style |
| [getBorderStyle()](#getBorderStyle--) | Obtient la BorderStyle dans le style |
| [getBorderWidth()](#getBorderWidth--) | Obtient la BorderWidth dans le style |
| [getBottomBorderStyle()](#getBottomBorderStyle--) | Spécifie le style de la bordure inférieure de la cellule. |
| [getClass()](#getClass--) |  |
| [getCssClass()](#getCssClass--) | Obtient la CssClass dans le style |
| [getCustom()](#getCustom--) | Obtient le format personnalisé, null ou chaîne vide signifie aucun format personnalisé. |
| [getFont()](#getFont--) | Obtient la Font dans le style |
| [getForeColor()](#getForeColor--) | Obtient la ForeColor dans le style |
| [getHeight()](#getHeight--) | Obtient la Height dans le style |
| [getHorizontalAlign()](#getHorizontalAlign--) | Obtient le HorizontalAlign dans le style |
| [getIndentLevel()](#getIndentLevel--) | Obtient le niveau d'indentation. |
| [getLeftBorderStyle()](#getLeftBorderStyle--) | Spécifie le style de la bordure gauche de la cellule. |
| [getNumberType()](#getNumberType--) | Obtient le format d'affichage des nombres et des dates. |
| [getQuotePrefix()](#getQuotePrefix--) | Indique si la valeur de la cellule commence par une apostrophe. |
| [getRightBorderStyle()](#getRightBorderStyle--) | Spécifie le style de la bordure droite de la cellule. |
| [getRotationAngle()](#getRotationAngle--) | Obtient l'attribut Rotation. |
| [getTopBorderStyle()](#getTopBorderStyle--) | Spécifie le style de la bordure supérieure de la cellule. |
| [getVerticalAlign()](#getVerticalAlign--) | Obtient le VerticalAlign dans le style |
| [getWidth()](#getWidth--) | Obtient la Width dans le style |
| [getWrap()](#getWrap--) | Obtient le Wrap dans le style |
| [hashCode()](#hashCode--) | Servir de fonction de hachage pour un type particulier, adaptée à une utilisation dans les algorithmes de hachage et les structures de données comme une table de hachage. |
| [isLocked()](#isLocked--) | Obtient une valeur indiquant si une cellule peut être modifiée ou non lorsque sa feuille de calcul est protégée. |
| [mergeWith(WebStyle s)](#mergeWith-com.aspose.gridweb.WebStyle-) | Fusionne avec un autre objet de style. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBackColor(Color value)](#setBackColor-com.aspose.gridweb.Color-) | Définit le BackColor dans le style |
| [setBackImageAttributes(String value)](#setBackImageAttributes-java.lang.String-) | Attributs de l'image d'arrière-plan. |
| [setBackImageUrl(String value)](#setBackImageUrl-java.lang.String-) | URL de l'image d'arrière-plan. |
| [setBorderColor(Color value)](#setBorderColor-com.aspose.gridweb.Color-) | Définit le BorderColor dans le style |
| [setBorderStyle(int value)](#setBorderStyle-int-) | Définit le BorderStyle dans le style |
| [setBorderWidth(Unit value)](#setBorderWidth-com.aspose.gridweb.Unit-) | Définit le BorderWidth dans le style |
| [setBottomBorderStyle(WebBorderStyle value)](#setBottomBorderStyle-com.aspose.gridweb.WebBorderStyle-) | Spécifie le style de la bordure inférieure de la cellule. |
| [setCssClass(String value)](#setCssClass-java.lang.String-) | Définit le CssClass dans le style |
| [setCustom(String value)](#setCustom-java.lang.String-) | Définit le format personnalisé, null ou chaîne vide signifie aucun format personnalisé. |
| [setForeColor(Color value)](#setForeColor-com.aspose.gridweb.Color-) | Définit le ForeColor dans le style |
| [setHeight(Unit value)](#setHeight-com.aspose.gridweb.Unit-) | Définit la Height dans le style |
| [setHorizontalAlign(int value)](#setHorizontalAlign-int-) | Définit le HorizontalAlign dans le style |
| [setIndentLevel(int value)](#setIndentLevel-int-) | Définit le niveau d'indentation. |
| [setLeftBorderStyle(WebBorderStyle value)](#setLeftBorderStyle-com.aspose.gridweb.WebBorderStyle-) | Spécifie le style de la bordure gauche de la cellule. |
| [setLocked(boolean value)](#setLocked-boolean-) | Définit une valeur indiquant si une cellule peut être modifiée ou non lorsque sa feuille de calcul est protégée. |
| [setNumberType(int value)](#setNumberType-int-) | Définit le format d'affichage des nombres et des dates. |
| [setQuotePrefix(boolean value)](#setQuotePrefix-boolean-) | Indique si la valeur de la cellule commence par une apostrophe. |
| [setRightBorderStyle(WebBorderStyle value)](#setRightBorderStyle-com.aspose.gridweb.WebBorderStyle-) | Spécifie le style de la bordure droite de la cellule. |
| [setRotationAngle(short value)](#setRotationAngle-short-) | Définit l'attribut Rotation. |
| [setTopBorderStyle(WebBorderStyle value)](#setTopBorderStyle-com.aspose.gridweb.WebBorderStyle-) | Spécifie le style de la bordure supérieure de la cellule. |
| [setVerticalAlign(int value)](#setVerticalAlign-int-) | Définit le VerticalAlign dans le style |
| [setWidth(Unit value)](#setWidth-com.aspose.gridweb.Unit-) | Définit la Width dans le style |
| [setWrap(boolean value)](#setWrap-boolean-) | Définit le Wrap dans le style |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridTableItemStyle() {#GridTableItemStyle--}
```
public GridTableItemStyle()
```


Constructeur par défaut.

### copyFrom(WebStyle s) {#copyFrom-com.aspose.gridweb.WebStyle-}
```
public void copyFrom(WebStyle s)
```


Copie à partir d'un autre objet de style.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| s | [WebStyle](../../com.aspose.gridweb/webstyle) | un autre objet de style |

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
### getBackColor() {#getBackColor--}
```
public Color getBackColor()
```


Obtient la BackColor dans le style

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getBackImageAttributes() {#getBackImageAttributes--}
```
public String getBackImageAttributes()
```


Attributs de l'image d'arrière-plan.

**Returns:**
java.lang.String
### getBackImageUrl() {#getBackImageUrl--}
```
public String getBackImageUrl()
```


URL de l'image d'arrière-plan.

**Returns:**
java.lang.String
### getBorderColor() {#getBorderColor--}
```
public Color getBorderColor()
```


Obtient la BorderColor dans le style

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getBorderStyle() {#getBorderStyle--}
```
public int getBorderStyle()
```


Obtient la BorderStyle dans le style

Voir [BorderStyle](../../com.aspose.gridweb/borderstyle).

**Returns:**
int
### getBorderWidth() {#getBorderWidth--}
```
public Unit getBorderWidth()
```


Obtient la BorderWidth dans le style

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getBottomBorderStyle() {#getBottomBorderStyle--}
```
public WebBorderStyle getBottomBorderStyle()
```


Spécifie le style de la bordure inférieure de la cellule.

**Returns:**
[WebBorderStyle](../../com.aspose.gridweb/webborderstyle)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCssClass() {#getCssClass--}
```
public String getCssClass()
```


Obtient la CssClass dans le style

**Returns:**
java.lang.String
### getCustom() {#getCustom--}
```
public String getCustom()
```


Obtient le format personnalisé, null ou chaîne vide signifie aucun format personnalisé.

**Returns:**
java.lang.String
### getFont() {#getFont--}
```
public FontInfo getFont()
```


Obtient la Font dans le style

**Returns:**
[FontInfo](../../com.aspose.gridweb/fontinfo)
### getForeColor() {#getForeColor--}
```
public Color getForeColor()
```


Obtient la ForeColor dans le style

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getHeight() {#getHeight--}
```
public Unit getHeight()
```


Obtient la Height dans le style

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getHorizontalAlign() {#getHorizontalAlign--}
```
public int getHorizontalAlign()
```


Obtient le HorizontalAlign dans le style

Voir [HorizontalAlign](../../com.aspose.gridweb/horizontalalign).

**Returns:**
int
### getIndentLevel() {#getIndentLevel--}
```
public int getIndentLevel()
```


Obtient le niveau d'indentation.

**Remarks**

**Returns:**
int
### getLeftBorderStyle() {#getLeftBorderStyle--}
```
public WebBorderStyle getLeftBorderStyle()
```


Spécifie le style de la bordure gauche de la cellule.

**Returns:**
[WebBorderStyle](../../com.aspose.gridweb/webborderstyle)
### getNumberType() {#getNumberType--}
```
public int getNumberType()
```


Obtient le format d'affichage des nombres et des dates. Les modèles de formatage diffèrent selon les régions.

**Remarks**

Par exemple, les modèles de formatage représentés par des nombres pour la région en\\_US :

| Valeur | Type | Chaîne de format |
| ----- | ---------- | ---------------------------------------------------- |
| 0 | General | `General` |
| 1 | Decimal | `0` |
| 2 | Decimal | `0.00` |
| 3 | Decimal | `#,##0` |
| 4 | Decimal | `#,##0.00` |
| 5 | Currency | `$#,##0_);($#,##0)` |
| 6 | Currency | `$#,##0_);[Rouge](../$#,##0)` |
| 7 | Currency | `$#,##0.00_);($#,##0.00)` |
| 8 | Currency | `$#,##0.00_);[Rouge](../$#,##0.00)` |
| 9 | Percentage | `0%` |
| 10 | Percentage | `0.00%` |
| 11 | Scientific | `0.00E+00` |
| 12 | Fraction | `# ?/?` |
| 13 | Fraction | `# ??/??` |
| 14 | Date | `jj/mm/aaaa` |
| 15 | Date | `jj-mmm-aa` |
| 16 | Date | `jj-mmm` |
| 17 | Date | `mmm-aa` |
| 18 | Time | `hh:mm` |
| 19 | Time | `hh:mm:ss` |
| 20 | Time | `hh:mm` |
| 21 | Time | `hh:mm:ss` |
| 22 | Time | `jj/mm/aaaa hh:mm` |
| 37 | Accounting | `#,##0_);(#,##0)` |
| 38 | Accounting | `#,##0_);[Rouge](../#,##0)` |
| 39 | Accounting | `#,##0.00_);(#,##0.00)` |
| 40 | Accounting | `#,##0.00_);[Rouge](../#,##0.00)` |
| 41 | Accounting | `_(* #,##0_);_(* (#,##0);_(* "-"_);_(@_)` |
| 42 | Currency | `_($* #,##0_);_($* (#,##0);_($* "-"_);_(@_)` |
| 43 | Accounting | `_(* #,##0.00_);_(* (#,##0.00);_(* "-"??_);_(@_)` |
| 44 | Currency | `_($* #,##0.00_);_($* (#,##0.00);_($* "-"??_);_(@_)` |
| 45 | Time | `mm:ss` |
| 46 | Time | `[h]:mm:ss` |
| 47 | Time | `mm:ss.0` |
| 48 | Scientific | `##0.0E+0` |
| 49 | Text | `@` |

**Returns:**
int
### getQuotePrefix() {#getQuotePrefix--}
```
public boolean getQuotePrefix()
```


Indique si la valeur de la cellule commence par une apostrophe.

**Returns:**
boolean
### getRightBorderStyle() {#getRightBorderStyle--}
```
public WebBorderStyle getRightBorderStyle()
```


Spécifie le style de la bordure droite de la cellule.

**Returns:**
[WebBorderStyle](../../com.aspose.gridweb/webborderstyle)
### getRotationAngle() {#getRotationAngle--}
```
public short getRotationAngle()
```


Obtient l'attribut Rotation.

**Remarks**

0: Non pivoté.

255: De haut en bas.

\-90: Vers le bas.

90: Vers le haut.

Vous pouvez définir 255 ou une valeur comprise entre -90 et 90.

**Returns:**
short
### getTopBorderStyle() {#getTopBorderStyle--}
```
public WebBorderStyle getTopBorderStyle()
```


Spécifie le style de la bordure supérieure de la cellule.

**Returns:**
[WebBorderStyle](../../com.aspose.gridweb/webborderstyle)
### getVerticalAlign() {#getVerticalAlign--}
```
public int getVerticalAlign()
```


Obtient le VerticalAlign dans le style

Voir [VerticalAlign](../../com.aspose.gridweb/verticalalign).

**Returns:**
int
### getWidth() {#getWidth--}
```
public Unit getWidth()
```


Obtient la Width dans le style

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getWrap() {#getWrap--}
```
public boolean getWrap()
```


Obtient le Wrap dans le style

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public int hashCode()
```


Servir de fonction de hachage pour un type particulier, adaptée à une utilisation dans les algorithmes de hachage et les structures de données comme une table de hachage.

**Returns:**
int - Un code de hachage pour le style actuel.
### isLocked() {#isLocked--}
```
public boolean isLocked()
```


Obtient une valeur indiquant si une cellule peut être modifiée ou non lorsque sa feuille de calcul est protégée. Lorsque la feuille de calcul est protégée et que IsLocked est vrai, la cellule ne peut pas être modifiée. Lorsque la feuille de calcul est protégée et que IsLocked est faux, la cellule peut être modifiée.

**Returns:**
boolean
### mergeWith(WebStyle s) {#mergeWith-com.aspose.gridweb.WebStyle-}
```
public void mergeWith(WebStyle s)
```


Fusionne avec un autre objet de style.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| s | [WebStyle](../../com.aspose.gridweb/webstyle) | un autre objet de style |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setBackColor(Color value) {#setBackColor-com.aspose.gridweb.Color-}
```
public void setBackColor(Color value)
```


Définit le BackColor dans le style

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setBackImageAttributes(String value) {#setBackImageAttributes-java.lang.String-}
```
public void setBackImageAttributes(String value)
```


Attributs de l'image d'arrière-plan.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setBackImageUrl(String value) {#setBackImageUrl-java.lang.String-}
```
public void setBackImageUrl(String value)
```


URL de l'image d'arrière-plan.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setBorderColor(Color value) {#setBorderColor-com.aspose.gridweb.Color-}
```
public void setBorderColor(Color value)
```


Définit le BorderColor dans le style

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setBorderStyle(int value) {#setBorderStyle-int-}
```
public void setBorderStyle(int value)
```


Définit le BorderStyle dans le style

Voir [BorderStyle](../../com.aspose.gridweb/borderstyle).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setBorderWidth(Unit value) {#setBorderWidth-com.aspose.gridweb.Unit-}
```
public void setBorderWidth(Unit value)
```


Définit le BorderWidth dans le style

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setBottomBorderStyle(WebBorderStyle value) {#setBottomBorderStyle-com.aspose.gridweb.WebBorderStyle-}
```
public void setBottomBorderStyle(WebBorderStyle value)
```


Spécifie le style de la bordure inférieure de la cellule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) |  |

### setCssClass(String value) {#setCssClass-java.lang.String-}
```
public void setCssClass(String value)
```


Définit le CssClass dans le style

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setCustom(String value) {#setCustom-java.lang.String-}
```
public void setCustom(String value)
```


Définit le format personnalisé, null ou chaîne vide signifie aucun format personnalisé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setForeColor(Color value) {#setForeColor-com.aspose.gridweb.Color-}
```
public void setForeColor(Color value)
```


Définit le ForeColor dans le style

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setHeight(Unit value) {#setHeight-com.aspose.gridweb.Unit-}
```
public void setHeight(Unit value)
```


Définit la Height dans le style

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setHorizontalAlign(int value) {#setHorizontalAlign-int-}
```
public void setHorizontalAlign(int value)
```


Définit le HorizontalAlign dans le style

Voir [HorizontalAlign](../../com.aspose.gridweb/horizontalalign).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setIndentLevel(int value) {#setIndentLevel-int-}
```
public void setIndentLevel(int value)
```


Définit le niveau d'indentation.

**Remarks**

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setLeftBorderStyle(WebBorderStyle value) {#setLeftBorderStyle-com.aspose.gridweb.WebBorderStyle-}
```
public void setLeftBorderStyle(WebBorderStyle value)
```


Spécifie le style de la bordure gauche de la cellule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


Définit une valeur indiquant si une cellule peut être modifiée ou non lorsque sa feuille de calcul est protégée. Lorsque la feuille de calcul est protégée et que IsLocked est vrai, la cellule ne peut pas être modifiée. Lorsque la feuille de calcul est protégée et que IsLocked est faux, la cellule peut être modifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setNumberType(int value) {#setNumberType-int-}
```
public void setNumberType(int value)
```


Définit le format d'affichage des nombres et des dates. Les modèles de formatage diffèrent selon les régions.

**Remarks**

Par exemple, les modèles de formatage représentés par des nombres pour la région en\\_US :

| Valeur | Type | Chaîne de format |
| ----- | ---------- | ---------------------------------------------------- |
| 0 | General | `General` |
| 1 | Decimal | `0` |
| 2 | Decimal | `0.00` |
| 3 | Decimal | `#,##0` |
| 4 | Decimal | `#,##0.00` |
| 5 | Currency | `$#,##0_);($#,##0)` |
| 6 | Currency | `$#,##0_);[Rouge](../$#,##0)` |
| 7 | Currency | `$#,##0.00_);($#,##0.00)` |
| 8 | Currency | `$#,##0.00_);[Rouge](../$#,##0.00)` |
| 9 | Percentage | `0%` |
| 10 | Percentage | `0.00%` |
| 11 | Scientific | `0.00E+00` |
| 12 | Fraction | `# ?/?` |
| 13 | Fraction | `# ??/??` |
| 14 | Date | `jj/mm/aaaa` |
| 15 | Date | `jj-mmm-aa` |
| 16 | Date | `jj-mmm` |
| 17 | Date | `mmm-aa` |
| 18 | Time | `hh:mm` |
| 19 | Time | `hh:mm:ss` |
| 20 | Time | `hh:mm` |
| 21 | Time | `hh:mm:ss` |
| 22 | Time | `jj/mm/aaaa hh:mm` |
| 37 | Accounting | `#,##0_);(#,##0)` |
| 38 | Accounting | `#,##0_);[Rouge](../#,##0)` |
| 39 | Accounting | `#,##0.00_);(#,##0.00)` |
| 40 | Accounting | `#,##0.00_);[Rouge](../#,##0.00)` |
| 41 | Accounting | `_(* #,##0_);_(* (#,##0);_(* "-"_);_(@_)` |
| 42 | Currency | `_($* #,##0_);_($* (#,##0);_($* "-"_);_(@_)` |
| 43 | Accounting | `_(* #,##0.00_);_(* (#,##0.00);_(* "-"??_);_(@_)` |
| 44 | Currency | `_($* #,##0.00_);_($* (#,##0.00);_($* "-"??_);_(@_)` |
| 45 | Time | `mm:ss` |
| 46 | Time | `[h]:mm:ss` |
| 47 | Time | `mm:ss.0` |
| 48 | Scientific | `##0.0E+0` |
| 49 | Text | `@` |

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setQuotePrefix(boolean value) {#setQuotePrefix-boolean-}
```
public void setQuotePrefix(boolean value)
```


Indique si la valeur de la cellule commence par une apostrophe.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setRightBorderStyle(WebBorderStyle value) {#setRightBorderStyle-com.aspose.gridweb.WebBorderStyle-}
```
public void setRightBorderStyle(WebBorderStyle value)
```


Spécifie le style de la bordure droite de la cellule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) |  |

### setRotationAngle(short value) {#setRotationAngle-short-}
```
public void setRotationAngle(short value)
```


Définit l'attribut Rotation.

**Remarks**

0: Non pivoté.

255: De haut en bas.

\-90: Vers le bas.

90: Vers le haut.

Vous pouvez définir 255 ou une valeur comprise entre -90 et 90.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | short |  |

### setTopBorderStyle(WebBorderStyle value) {#setTopBorderStyle-com.aspose.gridweb.WebBorderStyle-}
```
public void setTopBorderStyle(WebBorderStyle value)
```


Spécifie le style de la bordure supérieure de la cellule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) |  |

### setVerticalAlign(int value) {#setVerticalAlign-int-}
```
public void setVerticalAlign(int value)
```


Définit le VerticalAlign dans le style

Voir [VerticalAlign](../../com.aspose.gridweb/verticalalign).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setWidth(Unit value) {#setWidth-com.aspose.gridweb.Unit-}
```
public void setWidth(Unit value)
```


Définit la Width dans le style

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setWrap(boolean value) {#setWrap-boolean-}
```
public void setWrap(boolean value)
```


Définit le Wrap dans le style

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

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

