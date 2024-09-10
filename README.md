<!-- camera.html -->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Camera Access</title>
</head>
<body>
    <h1>Permiso para acceder a la cámara</h1>
    <button id="start-camera">Acceder a la cámara</button>
    <video id="camera-stream" width="640" height="480" autoplay></video>

    <script>
        document.getElementById('start-camera').addEventListener('click', async () => {
            try {
                const stream = await navigator.mediaDevices.getUserMedia({ video: true });
                document.getElementBy
