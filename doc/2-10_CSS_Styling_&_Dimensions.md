# jQuery ���ģ�CSS����ʽ���ߴ�

[TOC]

jQuery ������һ�������ķ�������ȡ������Ԫ�ص� CSS ���ԣ�

```js
// Getting CSS Properties:
$('h1').css('fontSize');
$('h1').css('font-size');
```

```js
// Setting CSS Properties:
$('h1').css('fontSize', '100px');
$('h1').css({
    fontSize: '100px',
    color: 'red'
});
```

ע��ڶ��������Ĳ�������ʽ����һ�����ж�����ԵĶ�������һ���������������ݶ�����ķ������� jQuery ������������������ܶ�����һ�������ö��ֵ��

������˵� CSS ��ʽ�� JavaScript ��ͨ����Ҫת��Ϊ�շ�д�������磬�� CSS ��ʽ `font-size` �� JavaScript ����һ����������ʱ��ᱻд�� `fontSize`�������������ַ�����ʽ����һ�� CSS ���Ը�������������ʱ�򲻻���Ӱ�죬����������£��շ�д���ͺ��д�����������á�

�����Ƽ������������н� `.css()` ��Ϊһ��������ʹ�ã����ǵ�����һ������������ CSS ��ʱ��CSS ���Ի����շ�д�������Ǻ��д����

## ʹ�� CSS ����������ʽ
��Ϊһ����ȡ����`.css()` �����Ǻ��м�ֵ�ġ����ǣ���һ����Ҫ�����������б�����Ϊһ��������ʹ�ã���Ϊһ����ñ���չ�ֵ���Ϣ�� JavaScript ����֮�⡣�෴����д CSS �������������������Ӿ�״̬��Ȼ���޸�Ԫ�ص��ࡣ

```js
// Working with classes.
 
var h1 = $('h1');
 
h1.addClass('big');
h1.removeClass('big');
h1.toggleClass('big');
 
if ( h1.hasClass('big') ) {
    ...
}
```

�໹������������Ԫ�ص�״̬��Ϣ����������һ��Ԫ�ر�ѡ��

## �ߴ�
jQuery  �ṩ�˸�ʽ�����ķ�������ȡ���޸�Ԫ�سߴ��λ�á�

����Ĵ���� jQuery �еĳߴ繦������һ����̵�չʾ��

```js
// Basic dimensions methods.
 
// Sets the width of all <h1> elements.
$( "h1" ).width( "50px" );
 
// Gets the width of the first <h1> element.
$( "h1" ).width();
 
// Sets the height of all <h1> elements.
$( "h1" ).height( "50px" );
 
// Gets the height of the first <h1> element.
$( "h1" ).height();
 
 
// Returns an object containing position information for
// the first <h1> relative to its "offset (positioned) parent".
$( "h1" ).position();
```