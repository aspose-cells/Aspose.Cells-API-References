---
title: "DefaultStyleSettings Class"
linktitle: "DefaultStyleSettings"
articleTitle: "DefaultStyleSettings"
second_title: "Aspose.Cells for PHP via Java"
description: "Settings for the default values of workbook's style properties."
type: docs
weight: 1700
url: /php/aspose.cells/defaultstylesettings/
---

## DefaultStyleSettings class

Settings for the default values of workbook's style properties.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [BuiltInPreference](#builtinpreference) | boolean | Indicates whether property for number format is preferrable when the style defines both built-in number and custom patte |
| [FontName](#fontname) | String | Gets/Sets the default font name for the workbook |
| [FontSize](#fontsize) | Number | Gets/Sets the default standard font size for the workbook. |
| [HorizontalAlignment](#horizontalalignment) | Number | Gets/Sets the default value for horizontal alignment The value of the property is TextAlignmentType integer constant. |
| [VerticalAlignment](#verticalalignment) | Number | Gets/Sets the default value for vertical alignment The value of the property is TextAlignmentType integer constant. |

### DefaultStyleSettings.BuiltInPreference property {#builtinpreference}

Indicates whether property for number format is preferrable when the style defines both built-in number and custom pattern. Default value is false, that means by default custom pattern will be used to format values as long as it is not empty for one style. When loading workbook from existing template file, maybe both built-in number and custom pattern are defined for one style. This property determine whether we should use the built-in number or the custom pattern when formatting values with the style.

**Type:** boolean

### DefaultStyleSettings.FontName property {#fontname}

Gets/Sets the default font name for the workbook

**Type:** String

### DefaultStyleSettings.FontSize property {#fontsize}

Gets/Sets the default standard font size for the workbook.

**Type:** Number

### DefaultStyleSettings.HorizontalAlignment property {#horizontalalignment}

Gets/Sets the default value for horizontal alignment The value of the property is TextAlignmentType integer constant.

**Type:** Number

### DefaultStyleSettings.VerticalAlignment property {#verticalalignment}

Gets/Sets the default value for vertical alignment The value of the property is TextAlignmentType integer constant.

**Type:** Number
