<!DOCTYPE html>
<html lang="ar">
<head>
  <meta charset="UTF-8">
  <title>نابليون بونابرت</title>
  <style>
    body {
      margin: 0;
      padding: 20px;
      background: black;
      color: gold;
      font-family: Arial, sans-serif;
      text-align: center;
    }
    h1 {
      font-size: 2.5em;
      margin-bottom: 20px;
    }
    p {
      font-size: 1.5em;
      line-height: 1.8;
    }
    .box {
      border: 2px solid gold;
      padding: 20px;
      border-radius: 15px;
      background: rgba(255, 215, 0, 0.05);
      display: inline-block;
      max-width: 600px;
    }
  </style>
</head>
<body>
  <div class="box">
    <h1 id="title">نابليون بونابرت</h1>
    <p id="text">كان نابليون واحد من أعظم القادة العسكريين في التاريخ.</p>
  </div>

  <script>
    const data = [
      {
        title: "نابليون بونابرت",
        text: "كان نابليون واحد من أعظم القادة العسكريين في التاريخ."
      },
      {
        title: "الحملة على مصر",
        text: "قاد نابليون حملة على مصر عام 1798 وكان لها تأثير كبير على المنطقة."
      },
      {
        title: "إمبراطور فرنسا",
        text: "توّج نابليون نفسه إمبراطورًا على فرنسا سنة 1804."
      },
      {
        title: "نهايته",
        text: "نُفي نابليون إلى جزيرة سانت هيلينا بعد هزيمته في معركة واترلو وتوفي هناك."
      }
    ];

    let index = 0;
    document.body.onkeyup = function(e){
      if(e.code === "Space") {
        index = (index + 1) % data.length;
        document.getElementById("title").innerText = data[index].title;
        document.getElementBy
