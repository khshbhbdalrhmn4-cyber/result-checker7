<!DOCTYPE html>
<html>
<head>
  <title>درجة الطالب</title>
  <meta charset="UTF-8">
</head>
<body style="font-family: sans-serif; text-align: center; margin-top: 100px;">
  <h2>احسب تقديرك 🎓</h2>
  <input type="number" id="mark" placeholder="اكتب درجتك" style="padding: 10px; font-size: 16px;">
  <button onclick="calcGrade()" style="padding: 10px 20px; margin-left: 10px; font-size: 16px;">اعرف التقدير</button>
  <p id="result" style="font-size: 20px; margin-top: 20px;"></p>

  <script>
    function calcGrade() {
      let mark = document.getElementById("mark").value;
      let grade;

      if (mark >= 90 && mark <= 100) grade = "A";
      else if (mark >= 80 && mark < 90) grade = "B";
      else if (mark >= 70 && mark < 80) grade = "C";
      else if (mark >= 60 && mark < 70) grade = "D";
      else grade = "Fail";

      document.getElementById("result").innerText = "تقديرك هو: " + grade;
    }
  </script>
</body>
</html>
