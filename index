<!DOCTYPE html>
<html>
<head>
  <meta charset="UTF-8">
  <title>SERYFA League Tables</title>
  <style>
    html, body {
      margin: 0;
      padding: 0;
      font-family: Arial, sans-serif;
      height: 100%;
    }
    header {
      padding: 10px;
      background: #FFD700;
      text-align: center;
    }
    select {
      font-size: 16px;
      padding: 6px 10px;
      margin-top: 10px;
    }
    iframe {
      width: 100%;
      height: calc(100vh - 60px);
      border: none;
    }
  </style>
</head>
<body>
  <header>
    <h2>SERYFA League Tables</h2>
    <label for="ageGroup">Select Age Group: </label>
    <select id="ageGroup">
      <option value="U13">U13</option>
      <option value="U14">U14</option>
      <option value="U15">U15</option>
      <option value="U16">U16</option>
      <option value="U17">U17</option>
      <option value="U18">U18</option>
    </select>
  </header>

  <iframe id="leagueFrame" src=""></iframe>

  <script>
    const iframe = document.getElementById("leagueFrame");
    const selector = document.getElementById("ageGroup");

    function loadAgeGroup(age) {
      const baseUrl = "https://script.google.com/macros/s/AKfycbyvH39UniVB2NIQ0dPjdTxJLqP3CvtJRcaFIxZLCukw7m7OgI00iv8eTvT48ZEG8lEDnA/exec";
      iframe.src = `${baseUrl}?ageGroup=${age}`;
    }

    selector.addEventListener("change", () => {
      loadAgeGroup(selector.value);
    });

    // Load default age group (U13) on page load
    window.onload = () => {
      loadAgeGroup(selector.value);
    };
  </script>
</body>
</html>
