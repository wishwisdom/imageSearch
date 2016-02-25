# Google Custom Search API 를 이용한 Image 검색

var cx = '017643444788069204610:4gvhea_mvga'; /
var gcse = document.createElement('script'); gcse.type = 'text/javascript';

gcse.async = true;
gcse.src = 'https://cse.google.com/cse.js?cx=' + cx;

var s = document.getElementsByTagName('script')[0]; 
s.parentNode.insertBefore(gcse, s);
})();

cx는 google에서 제공해주는 Google Search engine ID이며,

ID를 생성할 때 설정한, 검색을 할 URL로 설정된 engine


google에서 제공해주는 form을 랜더링하는 부분.
div: "test" -> 랜더링을 할 target tag id
tag: 'search' -> search tag form 생성
attributes -> 공식 사이트에서 제공해주는 option을 주는 부분
	disableWebSearch -> image 검색만 할 수 있도록 "true"로 둠.

google.search.cse.element.render({
    div: "test",	// renderring할 div tag id
    tag: 'search'	// search tag를 생성
    attributes:{
        disableWebSearch: "true"	// 이미지를 제외한 모든 검색결과 제외
     }
});

