Selectors�G
http://www.w3schools.com/cssref/css_selectors.asp
http://www.w3schools.com/css/css_attribute_selectors.asp
Demo�G

��ܾ�(Selectors)�A�]�wStyle��H�FCSS�O����w����H�]�w��˦��A�]����ܾ��O���A���e���ɤ�������(Element)�B���O(Class)�B�s��(ID)�B�ݩ�(Attribute)���j�M�A�Y�s�b�h��Ӥ���]�w�˦��C

�� Class

CSS�G
.xxx { ... }

HTML�G
<element class="xxx"> </element>

�YElement��class�ݩʦ����w��xxx�A�h�˹���˦��]�w�C

1. class���i�s���h��css�˦�
CSS�G
.xxx {...}
.yyy {...}

HTML�G
<element class"xxx yyy">

2. class�]�w�����h�S��
CSS�G
.xxx {...}
.xxx .subx {...}

HTML�G
<element class="xxx"> <element class="subx"> class "subx" will done. </element> </element>
<element class="yyy"> <element class="subx"> class "subx" not done. </element> </element>

�Y�]�����h�A�h�u�����ݩ󤺼h������]�wclass�~�|�˹��˦��F�Ϥ��h���|�˹��C

�� ID

CSS�G
#xxx { ... }

HTML�G
<element id="xxx"> </element>

�YElement��id�ݩʦ����w��xxx�A�h�˹���˦��]�w�C

1. ID�]�w�����h�S��
CSS�G
#xxx {...}
#xxx #subx {...}

HTML�G
<element id="xxx"> <element id="subx"> id "subx" will done. </element> </element>
<element id="yyy"> <element id="subx"> id "subx" not done. </element> </element>

�Y�]�����h�A�h�u�����ݩ󤺼h������]�wclass�~�|�˹��˦��F�Ϥ��h���|�˹��C

�� Element

CSS�G
xxx { ... }

HTML�G
<xxx> </xxx>

�YElement�����w��xxx�A�h�˹���˦��]�w�C

1. ���w�ŦX��class�PID
CSS�G
element.xxx{...}
element#yyy {...}

HTML�G
<element class="xxx"> class "xxx" will done. </element>
<element id="yyy"> id "yyy" will done. </element>

�� Attribute
http://www.w3schools.com/css/css_attribute_selectors.asp

CSS�G
element[attribute {op-code} value] { ... }

HTML�G
<element attribute="value"> </element>

�YElement����attribute�֦��ŦXop-code���w��value���e�A�h�˹���˦��]�w�C
��element�ëD���n�A�L�]�w�h��ܩҦ�element�A�Ϥ��h�w��S�welement�C
��op-code�Pvalue�ëD���n�A�L�]�w�h���attribute�s�b�Y�i�C

op-code
1. "="�Avalue�����ŦX
2. "~="�A�ƭȦ��ȲŦXvalue�F�����value�����Ϊťդ��}���h�ӭȡA�p attr="value1 value2"
3. "!="�A�ƭȫe�ݲŦXvalue�A�B��"-"�Ÿ��P��L���e���j�F�pattr="value-top1"
4. "^="�A�ƭȫe�ݲŦXvalue�A�L������Ÿ��P��L���e���j�F�pattr="valuetop1"
5. "$="�A�ƭȫ�ݲŦXvalue�A�L������Ÿ��P��L���e���j�F�pattr="topvalue"
6. "*="�A�ƭȤ��������ŦXvalue�A�L������Ÿ��P��L���e���j�F�pattr="top-value-x"

Pesudo-classes�G
http://www.w3schools.com/css/css_pseudo_classes.asp

selector:pseudo-class {
    property:value;
}

�Y��ܾ�(selector)�A�ŦX�Хܪ��A(pseudo-class)�A�˹���˦��C
���A�o�ͦh�Ӧ��s�������ƥ�B�[�c���A�A�̾ڤW�s�������C��Ѧҩһݪ����A�ӳ]�w�C

Box Model�G
http://www.w3schools.com/css/css_boxmodel.asp

�Ҧ�HTML����Ҧs���@��Boxes�A�bCSS���ABox model�Y�O�Q�׳]�p�P�W������Boxes�C
�p�W�夺�ҭz�A�@�Ӥ���i�Ϥ���U�C�|�h�A�Ѥ��ӥ~���C�|�G

1. Content�A���e����A�վ�e�B���ҬO�H���B����ǡC
2. Padding�A���ءA����Content�PBorder�������϶��C
3. Border�A��t�A��¶Padding���϶��A�q�`�Хܬ���u���ϰ�C
4. Margin�A�~�ءA����̥~�h�A�q�`�ΨӪ�ܬ����󶡪����Z�C

�@�Ӥ��󪺹�ڼe�B���A�O�N�W�z�|�h�[�`�Ӻ�FContent�~�A��l�T�h����A�Ҷq�W�U�B���k�A�Ҷ��⭿�p��C

Transitions�G
http://www.w3schools.com/css/css3_transitions.asp

CSS�ʵe�O���ݩʵo�ͧ��ܮɡA�g�Ѥ@�q�ɶ���~�N���ܰʨ���w�ȡC

���P��@��ʵe�O�ݭn��Ĳ�o����B�@�ACSS�ʵe�y�{�p�U�G
1. ��S�w�ؼЪ����w�ƭȳ]�w�ʵe�ƥ�ť�C
2. ��ť�ƭȡA�]�˦��]�w���ܦ��ܰʡAĲ�o�ഫ�ʵe�C

Ĳ�o�W�i�Ψ�ؤ覡�G
1. CSS Pesudo-classes
�露����w�F�ʵe�欰�A�é�Pesudo-classes�����w��ť�ƭ��ܧ�A�Ǧ�Ĳ�o�ʵe�C

2. JavaScript add class or setting style
��������w�F�ʵe�欰�A��JavaScript��ƹ��ɡA�露��W�[class�Χ���style�A�Ǧ�Ĳ�o�ʵe�C

-----------------------------------

Online Tools�G

CSS Type set
http://csstypeset.com/

pixels to em
http://pxtoem.com/

clean css
http://www.cleancss.com/?lang=en

make css menu
http://cssmenumaker.com/

Drawter
http://drawter.com/

CSS Portal�ACSS lib �U���P�d��
http://www.cssportal.com/animate-css/

Enjoy CSS�A�u�WCSS�]�w�u��
http://enjoycss.com/

CSS3 Maker�A�u�WCSS�]�w�u��
http://www.css3maker.com/