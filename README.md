# Sticky-Note-effect-with-html-css
.....html......
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width">
    <title>repl.it</title>
    <link href="style.css" rel="stylesheet" type="text/css" />
  </head>
  <body>
    <script src="script.js"></script>
    <ul>
  <li>
    <a href="#" contenteditable>
      <h2>Title #1</h2>
      <p>Shaaaaa...!</p>
    </a>
  </li>
  <li>
    <a href="#" contenteditable>
      <h2>Title #2</h2>
      <p>Isn't it lovely?</p>
    </a>
  </li>
  <li>
    <a href="#" contenteditable>
      <h2>Title #3</h2>
      <p>Top-notch</p>
    </a>
  </li>
  <li>
    <a href="#" contenteditable>
      <h2>Title #4</h2>
      <p>YoU got it!</p>
    </a>
  </li>
  <li>
    <a href="#" contenteditable>
      <h2>Title #5</h2>
      <p>Love that attitude</p>
    </a>
  </li>
  <li>
    <a href="#" contenteditable>
      <h2>Title #6</h2>
      <p>Excuse me!</p>
    </a>
  </li>
  <li>
    <a href="#" contenteditable>
      <h2>Title #7</h2>
      <p>Chill yaar..!</p>
    </a>
  </li>
  <li>
    <a href="#" contenteditable>
      <h2>Title #8</h2>
      <p>Far off!</p>
    </a>
  </li>
</ul>
  </body>
</html>
.....css......
body {
  margin: 20px auto;
  font-family: 'Lato';
  background:rgb(6, 214, 214);
  color:#fff;
}

*{
  margin:0;
  padding:0;
}

h2 {
  font-weight: bold;
  font-size: 2rem;
}
p {
  font-family: 'Reenie Beanie';
  font-size: 2rem;
}
ul,li{
  list-style:none;
}
ul{
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
}
ul li a{
  text-decoration:none;
  color:#000;
  background:rgb(197, 3, 171);
  display:block;
  height:10em;
  width:10em;
  padding:1em;
  box-shadow: 5px 5px 7px rgba(33,33,33,.7);
  transform: rotate(-6deg);
  transition: transform .15s linear;
}

ul li:nth-child(even) a{
  transform:rotate(4deg);
  position:relative;
  top:5px;
  background:rgb(133, 236, 101);
}
ul li:nth-child(3n) a{
  transform:rotate(-3deg);
  position:relative;
  top:-5px;
  background:rgb(190, 8, 17);
}
ul li:nth-child(5n) a{
  transform:rotate(5deg);
  position:relative;
  top:-10px;
}

ul li a:hover,ul li a:focus{
  box-shadow:10px 10px 7px rgba(0,0,0,.7);
  transform: scale(1.25);
  position:relative;
  z-index:5;
}

ul li{
  margin:1em;
}
