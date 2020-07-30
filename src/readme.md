## 基本觀念整理

### Selectors

+ [CSS Selectors](http://www.w3schools.com/cssref/css_selectors.asp)
+ [CSS Attribute Selectors](http://www.w3schools.com/css/css_attribute_selectors.asp)

選擇器(Selectors)，設定Style對象；CSS是對指定的對象設定其樣式，因此選擇器是指，對當前文檔內的元件(Element)、類別(Class)、編號(ID)、屬性(Attribute)等搜尋，若存在則對該元件設定樣式。

##### Class

CSS：
```
.xxx { ... }
```

HTML：
```
<element class="xxx"> </element>
```

若Element的class屬性有指定的xxx，則裝飾其樣式設定。

1. class內可存有多個css樣式

CSS：
```
.xxx {...}
.yyy {...}
```
HTML：
```
<element class"xxx yyy">
```

2. class設定有階層特性

CSS：
```
.xxx {...}
.xxx .subx {...}
```

HTML：
```
<element class="xxx"> <element class="subx"> class "subx" will done. </element> </element>
<element class="yyy"> <element class="subx"> class "subx" not done. </element> </element>
```

若設為階層，則只有隸屬於內層的元件設定class才會裝飾樣式；反之則不會裝飾。

##### ID

CSS：
```
#xxx { ... }
```

HTML：
```
<element id="xxx"> </element>
```

若Element的id屬性有指定的xxx，則裝飾其樣式設定。

1. ID設定有階層特性
CSS：
```
#xxx {...}
#xxx #subx {...}
```

HTML：
```
<element id="xxx"> <element id="subx"> id "subx" will done. </element> </element>
<element id="yyy"> <element id="subx"> id "subx" not done. </element> </element>
```

若設為階層，則只有隸屬於內層的元件設定class才會裝飾樣式；反之則不會裝飾。

##### Element

CSS：
```
xxx { ... }
```

HTML：
```
<xxx> </xxx>
```

若Element為指定的xxx，則裝飾其樣式設定。

1. 指定符合的class與ID
CSS：
```
element.xxx{...}
element#yyy {...}
```

HTML：
```
<element class="xxx"> class "xxx" will done. </element>
<element id="yyy"> id "yyy" will done. </element>
```

##### Attribute

CSS：
```
element[attribute {op-code} value] { ... }
```

HTML：
```
<element attribute="value"> </element>
```

若Element內的attribute擁有符合op-code指定的value內容，則裝飾其樣式設定。
※element並非必要，無設定則表示所有element，反之則針對特定element。
※op-code與value並非必要，無設定則表示attribute存在即可。

op-code
1. "="，value完全符合
2. "~="，數值有值符合value；此表示value內有用空白分開的多個值，如 attr="value1 value2"
3. "!="，數值前端符合value，且用"-"符號與其他內容分隔；如attr="value-top1"
4. "^="，數值前端符合value，無須任何符號與其他內容分隔；如attr="valuetop1"
5. "$="，數值後端符合value，無須任何符號與其他內容分隔；如attr="topvalue"
6. "\*="，數值內有部分符合value，無須任何符號與其他內容分隔；如attr="top-value-x"

##### [CSS Pesudo-classes](http://www.w3schools.com/css/css_pseudo_classes.asp)

```
selector:pseudo-class {
    property:value;
}
```

若選擇器(selector)，符合標示狀態(pseudo-class)，裝飾其樣式。
狀態發生多來自瀏覽器的事件、架構狀態，依據上連結內的列表參考所需的狀態來設定。

##### [Box Model](http://www.w3schools.com/css/css_boxmodel.asp)

所有HTML元件皆存有一個Boxes，在CSS中，Box model即是討論設計與規劃元件的Boxes。
如上文內所述，一個元件可區分文下列四層，由內而外的列舉：

1. Content，內容本文，調整寬、高皆是以此處為基準。
2. Padding，內框，介於Content與Border之間的區塊。
3. Border，邊緣，環繞Padding的區塊，通常標示為邊線的區域。
4. Margin，外框，元件最外層，通常用來表示為元件間的間距。

一個元件的實際寬、高，是將上述四層加總來算；Content外，其餘三層為邊，考量上下、左右，皆須兩倍計算。

##### [Transitions](http://www.w3schools.com/css/css3_transitions.asp)

CSS動畫是當屬性發生改變時，經由一段時間後才將值變動到指定值。

不同於一般動畫是需要時觸發物件運作，CSS動畫流程如下：
1. 對特定目標的指定數值設定動畫事件偵聽。
2. 偵聽數值，因樣式設定改變而變動，觸發轉換動畫。

觸發上可用兩種方式：
1. CSS Pesudo-classes
對元件指定了動畫行為，並於Pesudo-classes內指定偵聽數值變更，藉此觸發動畫。

2. JavaScript add class or setting style
隊元件指定了動畫行為，當JavaScript函數實行時，對元件增加class或改變style，藉此觸發動畫。
