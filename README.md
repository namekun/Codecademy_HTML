# Learn HTML by Codecademy

1. **HTML** stands for **H**yper**T**ext **M**arkup **L**anguage and is used to create the structure and content of a webpage.
2. Most HTML elements contain opening and closing tags with raw text or other HTML tags between them.
3. HTML elements can be nested inside other elements. The enclosed element is the child of the enclosing parent element.
4. Any visible content should be placed within the opening and closing `<body>` tags .
5. Headings and sub-headings, `<h1>` to `<h6>` tags, are used to enlarge text.
6. `<p>`, `<span>` and `<div>` tags specify text or blocks.
7. The `<em>(기울여쓰기)` and `<strong>(굵게쓰기)` tags are used to emphasize text.
8. Line breaks are created with the `<br>(한줄띄우기)` tag.
9. Ordered lists (`<ol>`) are numbered and unordered lists (`<ul>`) are bulleted.
10. Images (`<img>`) and videos (`<video>`) can be added by linking to an existing source.



Example )

```html
<body>

  <h1>The Brown Bear</h1>

  <div id="introduction">

    <h2>About Brown Bears</h2>

    <p>The brown bear (<em>Ursus arctos</em>) is native to parts of northern Eurasia and North America. Its conservation status is currently <strong>Least Concern</strong>.<br /><br /> There are many subspecies within the brown bear species, including the Atlas bear and the Himalayan brown bear.</p>

    <h3>Species</h3>

    <ul>

      <li>Arctos</li>

      <li>Collarus</li>

      <li>Horribilis</li>

      <li>Nelsoni (extinct)</li>

    </ul>

    <h3>Features</h3>

    <p>Brown bears are not always completely brown. Some can be reddish or yellowish. They have very large, curved claws and huge paws. Male brown bears are often 30% larger than female brown bears. They can range from 5 feet to 9 feet from head to toe.</p>

  </div>

  <div id="habitat">

    <h2>Habitat</h2>

    <h3>Countries with Large Brown Bear Populations</h3>

    <ol>

      <li>Russia</li>

      <li>United States</li>

      <li>Canada</li>

    </ol>

    <h3>Countries with Small Brown Bear Populations</h3>

    <p>Some countries with smaller brown bear populations include Armenia, Belarus, Bulgaria, China, Finland, France, Greece, India, Japan, Nepal, Poland, Romania, Slovenia, Turkmenistan, and Uzbekistan.</p>

  </div>

  <div id="media">

    <h2>Media</h2>
<img src="https://s3.amazonaws.com/codecademy-content/courses/web-101/web101-image_brownbear.jpg" alt="A Brown Bear"/>
    <video src ="https://s3.amazonaws.com/codecademy-content/courses/freelance-1/unit-1/lesson-2/htmlcss1-vid_brown-bear.mp4" width="320" height="240" controls>Video not supported</video>

  </div>

</body>
```



# [Learn HTML: Elements and Structure](https://www.codecademy.com/learn/learn-html)

1. HTML 문서를 작성하기 위해서 맨 처음에 `<!DOCTYPE html>`을 선언해줘야한다.

2. 페이지의 타이틀을 지정해 주기 위해 `<title></title>`안에 내용을 작성해준다.

3. 타 페이지로 통하는 링크를 걸어주기 위해서는 `<a href = "url"></a>`

   링크를 클릭했을때, 새 페이지에서 열기를 원한다면 `<a>`에 target = "_blank" 를 더해준다.

4. Relative Page로의 연결` <a href="./***.html"></a>` . 여기서 ./의 의미는 현재 폴더에서 파일을 찾음을 의미

5. 이미지를 눌러 사이트를 이동하게 하려면 `<a href ="url"></a>`로 <img=/>를 감싸준다.

6. 같은 페이지 안에 있는 부분으로 쉽게 이동하게 하기 위해서 리스트를 만들어준뒤(ol이건 ul이건 상관없다!) div의 id 부분을 다음과 같이 태그하면된다.

   `<li><a href="#div_id">내용</a></li>`

7. 들여쓰기를 할때에는 스페이스 두칸만큼 들여쓰기 합니다.

8. 주석은` <!--내용 -->`

###### Eng ver.

1. The `<!DOCTYPE html>` declaration should always be the first line of code in your HTML files. This lets the browser know what version of HTML to expect.
2. The `<html>` element will contain all of your HTML code.
3. Information about the web page, like the title, belongs within the `<head>` of the page.
4. You can add a title to your web page by using the `<title>` element, inside of the head.
5. A webpage's title appears in a browser's tab.
6. Anchor tags (`<a>`) are used to link to internal pages, external pages or content on the same page.
7. You can create sections on a webpage and jump to them using `<a>` tags and adding `id`s to the elements you wish to jump to.
8. Whitespace between HTML elements helps make code easier to read while not changing how elements appear in the browser.
9. Indentation also helps make code easier to read. It makes parent-child relationships visible.
10. Comments are written in HTML using the following syntax: `<!-- comment -->`.

# [Learn HTML: Tables](https://www.codecademy.com/learn/learn-html)

1. *Create table* 

   ```html
   <table></table>
   ```

2. *Table Rows*

   ```html
   <table>
       <tr></tr> <!--테이블의 로우를 만드는 명령어-->
   </table>
   ```

3. *Table Data*

   ```html
   <table>
       <tr>
       	<td>data</td>
       </tr>
   </table>
   ```

4. *Table Headings*

   ```html
   <table>
      	<tr>
       	<th>Heading</th>
       </tr> 
       <tr>
       	<td>data</td>
       </tr>
   </table>
   ```

5. *Table Borders*

   ```html
   <table border="1"> <!--Table의 테두리 같은것-->
     <tr>
       <td>73</td>
       <td>81</td>
     </tr>
   </table>
   ```

6. *colspan (spanning column)* - *숫자에 따라 그만큼 가로로 늘리는 것*

   ```html
   <table>
     <tr>
       <th>Month</th>
       <th>Savings</th>
     </tr>
     <tr>
       <td>January</td>
       <td>$100</td>
     </tr>
     <tr>
       <td>February</td>
       <td>$80</td>
     </tr>
     <tr>
       <td colspan="2">Sum: $180</td>
     </tr>
   </table>
   ```

7. *rowspan (Spanning Rows) - 수에 따라 그만큼 세로로 늘리는 것*

```html
<table>
  <tr> <!-- Row 1 -->
    <th></th>
    <th>Saturday</th>
    <th>Sunday</th>
  </tr>
  <tr> <!-- Row 2 -->
    <th>Morning</th>
    <td rowspan="2">Work</td>
    <td rowspan="3">Relax</td>
  </tr>
</table>
```

8.*Table Body *

*- The `<tbody>` element should contain all of the table's data, excluding the table headings*

*- 데이터 별로  행(row)그룹화 해주는 것이라고 생각하면 편하다!*

```html
<table>
  <tbody>
    <tr>
      <th></th>
      <th>Saturday</th>
      <th>Sunday</th>
    </tr>
    <tr>
      <th>Morning</th>
      <td rowspan="2">Work</td>
      <td rowspan="3">Relax</td>
    </tr>
   </tbody>
<table>
```

1. *Table Head*

*-thead 요소는 열의 제목으로 구성된 행의 그룹입니다.*

*-이 요소는 table 요소에서 한 번만 쓸 수 있으며, tbody나 tfoot보다 먼저 선언되어야 합니다.* 

```html
  <thead>
    <tr>
      <th>Company Name</th>
      <th>Number of Items to ship</th>
      <th>Next Action</th>
    </tr>
    </thead>
 	<tbody>
    <tr>
      <td colspan = "2">Adam's GreenWorks</td>
      <td rowspan = "2">14</td>
      <td>Package Items</td>
    </tr>
	</tbody>
```

1. *Table Footer*

*-tfoot 요소는 도표 하단에 나오는 열의 요약으로 구성된 행의 집합입니다.*

*-이 요소 역시 thead와 같이 table 내에 한 번만 쓸 수 있으며, tbody보다 먼저 작성하더라도 표의 맨 마지막에 위치하게 나옵니다.* 

```html
<table>
  <!-- tbody까지 생략 -->
  <tfoot>
    <tr>
      <td colspan="3">참가자 평균</td>
      <td>15.7</td>
      <td>35</td>
    </tr>
  </tfoot>
</table>
```

1. *Styling with CSS*

```css
table {
  height: 40%;
  left: 10%;
  margin: 20px auto;
  overflow-y: scroll;
  position: static;
  width: 80%;
}

thead th {
  background: #88CCF1;
  color: #FFF;
  font-family: 'Lato', sans-serif;
  font-size: 18px;
  font-weight: 100;
  letter-spacing: 2px;
  text-transform: uppercase;
}

tr {
  background: #f4f7f8;
  border-bottom: 1px solid #FFF;
  margin-bottom: 5px;
}

th, td {
  font-size: 18px;
  font-family: 'Lato', sans-serif;
  font-weight: 400;
  padding: 20px;
  text-align: left;
  width: 33.3333%;
}
```

1. *Final Code*

```html
<!DOCTYPE html>
<html>
<head>
  <title>Ship To It - Company Packing List</title>
  <link href="https://fonts.googleapis.com/css?family=Lato: 100,300,400,700|Luckiest+Guy|Oxygen:300,400" rel="stylesheet">
  <link href="style.css" type="text/css" rel="stylesheet">
</head>
<body>

  <ul class="navigation">
    <li><img src="https://s3.amazonaws.com/codecademy-content/courses/web-101/unit-9/htmlcss1-img_logo-shiptoit.png" height="20px;"></li>
    <li class="active">Action List</li>
    <li>Profiles</li>
    <li>Settings</li>
  </ul>

  <div class="search">Search the table</div>

  <table border="1">
    <thead>
    <tr>
      <th>Company Name</th>
      <th>Number of Items to ship</th>
      <th>Next Action</th>
    </tr>
    </thead>
    <tbody>
    <tr>
      <td colspan = "1">Adam's GreenWorks</td>
      <td rowspan = "1">14</td>
      <td>Package Items</td>
    </tr>
    <tr>
  <td>Davie's Burgers</td>
  <td>2</td>
  <td>Send Invoice</td>
</tr>
<tr>
  <td>Baker's Bike Shop</td>
  <td>3</td>
  <td>Send Invoice</td>
</tr>
<tr>
  <td>Miss Sally's Southern</td>
  <td>4</td>
  <td>Ship</td>
</tr>
<tr>
  <td>Summit Resort Rentals</td>
  <td>4</td>
  <td>Ship</td>
</tr>
    </tbody>
<tr>
  <td>Strike Fitness</td>
  <td>1</td>
  <td>Enter Order</td>
</tr>
    
   <tfoot>
    <td>Total</td>
 		<td>28</td>
    <td>null</td>
    </tfoot>
    
  </table>

</body>
</html>
```



## HTML Tables 정리

1. The `<table>` element creates a table.
2. The `<tr>` element adds rows to a table.
3. To add data to a row, you can use the `<td>`element.
4. Table headings clarify the meaning of data. Headings are added with the `<th>` element.
5. Table data can span columns using the `colspan`attribute.
6. Table data can span rows using the `rowspan`attribute.
7. Tables can be split into three main sections: a head, a body, and a footer.
8. A table's head is created with the `<thead>` element.
9. A table's body is created with the `<tbody>`element.
10. A table's footer is created with the `<tfoot>`element.
11. All the CSS properties you learned about in this course can be applied to tables and their data.
