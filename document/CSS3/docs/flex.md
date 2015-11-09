## flex

작성자 : 김동일

작성일 : 2015-10-27

css 레퍼런스 설명: 
 - flex : div 영역 내 모든 div tag를 같은 크기로 융통성있게 구분한다.
 
 - syntax : 
```sh 
flex: flex-grow flex-shrink flex-basis|auto|initial|inherit;
```

flex-grow : div로 구분되어 있는 항목 중 나머지 항목에 대하여 얼마나 늘릴 것인지 명시한다.

flex-shrink : div로 구분되어 있는 항목 중 나머지 항목에 대하여 얼마나 줄일 것인지 명시한다.

flex-basis : 영역 내 flex item 크기를 정의 한다. (auto, inherit, %, px, em 등)

auto : 기본 값인 1로 처리한다.

initial:기본 값으로 set되어 있는 값을 불러온다.(1)

none : 0으로 처리한다.

inherit:부모 element에 설정되어 있는 값을 상속 받는다.

sample code : 
```sh
<!DOCTYPE html>
<html>
<head>
<style> 
#main {
    width: 220px;
    height: 300px;
    border: 1px solid black;
    display: -webkit-flex; /* Safari */
    display: flex;
}

#main div {
    -webkit-flex: 1;  /* Safari 6.1+ */
    -ms-flex: 1;  /* IE 10 */    
    flex: 1;
}
</style>
</head>
<body>

<div id="main">
  <div style="background-color:coral;">RED</div>
  <div style="background-color:lightblue;">BLUE</div>  
  <div style="background-color:lightgreen;">Green div with more content.</div>
</div>

<p><b>Note:</b> Internet Explorer 9 and earlier versions do not support the flex property.</p>

<p><b>Note:</b> Internet Explorer 10 supports an alternative, the -ms-flex property. IE11 and newer versions fully support the flex property (do not need the -ms- prefix).</p>

<p><b>Note:</b> Safari 6.1 (and newer) supports an alternative, the -webkit-flex property.</p>

</body>
</html>

```

결과 

![flex](../images/flex.jpg)

### 목록
* [align-content](align-content.md)
* [align-items](align-items.md)
* [align-self](align-self.md)
* [@keyframes](@keyframes.md)
* [animation](animation.md)
* [animation-name](animation-name.md)
* [animation-duration](animation-duration.md)
* [animation-timing-function](animation-timing-function.md)
* [animation-delay](animation-delay.md)
* [animation-iteration-count](animation-iteration-count.md)
* [animation-direction](animation-direction.md)
* [animation-play-state](animation-play-state.md)
* [backface-visibility](backface-visibility.md)
* [background-clip](background-clip.md)
* [background-origin](background-origin.md)
* [background-size](background-size.md)
* [border-bottom-left-radius](border-bottom-left-radius.md)
* [border-bottom-right-radius](border-bottom-right-radius.md)
* [border-image](border-image.md)
* [border-image-outset](border-image-outset.md)
* [border-image-repeat](border-image-repeat.md)
* [border-image-slice](border-image-slice.md)
* [border-image-source](border-image-source.md)
* [border-image-width](border-image-width.md)
* [border-radius](border-radius.md)
* [border-top-left-radius](border-top-left-radius.md)
* [border-top-right-radius](border-top-right-radius.md)
* [box-shadow](box-shadow.md)
* [box-sizing](box-sizing.md)
* [column-count](column-count.md)
* [column-gap](column-gap.md)
* [column-rule](column-rule.md)
* [column-rule-color](column-rule-color.md)
* [column-rule-style](column-rule-style.md)
* [column-rule-width](column-rule-width.md)
* [column-span](column-span.md)
* [column-width](column-width.md)
* [columns](columns.md)
* [flex](flex.md)
* [flex-basis](flex-basis.md)
* [flex-direction](flex-direction.md)
* [flex-flow](flex-flow.md)
* [flex-grow](flex-grow.md)
* [flex-shrink](flex-shrink.md)
* [flex-wrap](flex-wrap.md)
* [@font-face](@font-face.md)
* [font-feature-settings](font-feature-settings.md)
* [hyphens](hyphens.md)
* [justify-content](justify-content.md)
* [opacity](opacity.md)
* [order](order.md)
* [outline-offset](outline-offset.md)
* [overflow-wrap](overflow-wrap.md)
* [overflow-x](overflow-x.md)
* [overflow-y](overflow-y.md)
* [perspective](perspective.md)
* [perspective-origin](perspective-origin.md)
* [resize](resize.md)
* [tab-size](tab-size.md)
* [text-align-last](text-align-last.md)
* [text-overflow](text-overflow.md)
* [text-shadow](text-shadow.md)
* [transform](transform.md)
* [transform-origin](transform-origin.md)
* [transform-style](transform-style.md)
* [transition](transition.md)
* [transition-delay](transition-delay.md)
* [transition-duration](transition-duration.md)
* [transition-property](transition-property.md)
* [transition-timing-function](transition-timing-function.md)
* [word-break](word-break.md)
* [word-wrap](word-wrap.md)