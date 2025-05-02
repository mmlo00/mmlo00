<!DOCTYPE html>
<html lang="ar">
<head>
  <meta charset="UTF-8">
  <title>نابليون بونابرت</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      font-family: 'Cairo', sans-serif;
      direction: rtl;
      background: linear-gradient(to bottom, #000, #1a1a1a);
      color: #f5f5f5;
      overflow: hidden;
    }

    .container {
      max-width: 800px;
      margin: 100px auto;
      padding: 30px;
      background: rgba(0, 0, 0, 0.6);
      border: 2px solid gold;
      border-radius: 20px;
      text-align: center;
      box-shadow: 0 0 30px rgba(255, 215, 0, 0.3);
      transition: all 0.7s ease;
      opacity: 1;
      transform: translateY(0);
    }

    h1 {
      font-size: 40px;
      color: gold;
      margin-bottom: 20px;
    }

    p {
      font-size: 24px;
      line-height: 1.8;
    }

    img {
      max-width: 100%;
      height: auto;
      border: 2px solid gold;
      border-radius: 15px;
      margin-top: 20px;
      box-shadow: 0 0 15px rgba(255, 215, 0, 0.4);
    }

    .fade-out {
      opacity: 0;
      transform: translateY(20px);
    }

    .fade-in {
      opacity: 1;
      transform: translateY(0);
    }
  </style>
</head>
<body>

  <div class="container fade-in" id="content">
    <h1>نابليون بونابرت</h1>
    <p>نابليون كان قائد عسكري فرنسي وإمبراطور فرنسا. وُلد في كورسيكا سنة 1769، وحقق شهرة سريعة بفضل عبقريته العسكرية.</p>
    <img src="https://i.imgur.com/V8uV1Xy.jpg" alt="نابليون">
  </div>

  <script>
    const data = [
      {
        title: "نابليون بونابرت",
        text: "نابليون كان قائد عسكري فرنسي وإمبراطور فرنسا. وُلد في كورسيكا سنة 1769، وحقق شهرة سريعة بفضل عبقريته العسكرية.",
        img: "https://i.imgur.com/V8uV1Xy.jpg"
      },
      {
        title: "معركة أوسترليتز (1805)",
        text: "أحد أعظم انتصارات نابليون، هزم فيها الجيوش الروسية والنمساوية، وأثبت قدرته على قيادة المعارك الحاسمة.",
        img: "https://i.imgur.com/T5IvxPS.jpg"
      },
      {
        title: "قوانين نابليون",
        text: "أصدر نابليون مجموعة من القوانين المعروفة بـ 'مدونة نابليون'، والتي أثرت على النظم القانونية في أوروبا.",
        img: "https://i.imgur.com/pYuvMG5.jpg"
      },
      {
        title: "نهاية الإمبراطورية",
        text: "بعد سلسلة من الهزائم، نُفي نابليون إلى جزيرة إلبا، ثم عاد لـ100 يوم قبل أن يُنفى أخيرًا إلى سانت هيلينا.",
        img: "https://i.imgur.com/ZnzQwZM.jpg"
      }
    ];

    let index = 0;
    const content = document.getElementById('content');

    document.addEventListener('keydown', (e) => {
      if (e.code === 'Space') {
        e.preventDefault();

        content.classList.remove('fade-in');
        content.classList.add('fade-out');

        setTimeout(() => {
          index = (index + 1) % data.length;
          content.innerHTML = `
            <h1>${data[index].title}</h1>
            <p>${data[index].text}</p>
            <img src="${data[index].img}" alt="${data[index].title}">
          `;
          content.classList.remove('fade-out');
          content.classList.add('fade-in');
        }, 500);
      }
    });
  </script>

</body>
</html>
