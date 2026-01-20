# yt
<!DOCTYPE html>
<html lang="zh">
<head>
  <meta charset="UTF-8" />
  <title>Animated Photo</title>
  <style>
    body {
      margin: 0;
      height: 100vh;
      background: #000;
      display: flex;
      justify-content: center;
      align-items: center;
      overflow: hidden;
    }

    .photo {
      width: 320px;
      border-radius: 16px;
      animation: breathe 6s ease-in-out infinite;
      box-shadow: 0 20px 40px rgba(0,0,0,0.5);
    }

    @keyframes breathe {
      0% {
        transform: scale(1) translateY(0);
      }
      50% {
        transform: scale(1.04) translateY(-6px);
      }
      100% {
        transform: scale(1) translateY(0);
      }
    }
  </style>
</head>
<body>
  <img src="photo.png" class="photo" />
</body>
</html>
