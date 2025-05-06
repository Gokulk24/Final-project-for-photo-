# Final-project-for-photo-
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Photo Viewer</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #111;
      color: #fff;
      text-align: center;
    }
    .viewer {
      margin: 50px auto;
      max-width: 800px;
    }
    #main-photo {
      width: 100%;
      max-height: 600px;
      object-fit: contain;
      border: 4px solid #fff;
    }
    .thumbnails {
      margin-top: 20px;
    }
    .thumbnails img {
      width: 100px;
      margin: 5px;
      cursor: pointer;
      border: 2px solid #444;
    }
    .thumbnails img:hover {
      border: 2px solid #fff;
    }
  </style>
</head>
<body>
  <h1>Photo Viewer</h1>
  <div class="viewer">
    <img id="main-photo" src="photo1.jpg" alt="Main Photo">
    <div class="thumbnails">
      <img src="photo1.jpg" onclick="changePhoto('photo1.jpg')" alt="">
      <img src="photo2.jpg" onclick="changePhoto('photo2.jpg')" alt="">
      <img src="photo3.jpg" onclick="changePhoto('photo3.jpg')" alt="">
    </div>
  </div>

  <script>
    function changePhoto(src) {
      document.getElementById('main-photo').src = src;
    }
  </script>
</body>
</html>
