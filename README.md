<!DOCTYPE html>
<html lang="en">

<head>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@4.3.1/dist/css/bootstrap.min.css"
        integrity="sha384-ggOyR0iXCbMQv3Xipma34MD+dH/1fQ784/j6cY/iJTQUOhcWr7x9JvoRxT2MZw1T" crossorigin="anonymous">
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Deuda a Gwensday</title>
    <link rel="icon" href="https://pm1.aminoapps.com/6956/9dc47d3201bb5b10ecc33b6c248fb617645f7a85r1-480-480v2_00.jpg">
</head>
<style>
    
</style>

<body style="background-color: black; overflow-x: hidden;">
    <video autoplay muted loop id="myVideo" style="width: 100%; height: 80%; position: absolute; margin-top: -10%;">
        <source src="videoplayback.mp4" type="video/mp4">
        Your browser does not support HTML5 video.
      </video>


    <div class="row justify-content-center" style="margin-top: 15%;">
        <div class="col-lg-6" style="text-align: center;">
            <h1 style="color: white; font-size: 40px; text-shadow: 3px 3px 3px black;">
                Anthony Actualmente debe aproximadamente unos:
            </h1>
            <div style="color: white; font-size: 100px; display: inline-flex; text-shadow: 3px 3px 3px black;">$
                <div id="value" style="color: white; font-size: 100px;text-shadow: 3px 3px 3px black;">0</div>
            </div>

            <div>
                <h1 style="color: white; font-size: 20px; text-shadow: 3px 3px 3px black;">
                    Siete Billones, noventa y dos millones, dieciséis mil trece Pesos
                </h1>
            </div>



        </div>

    </div>


    <!--javascript xd-->
    <script>
        function animateValue(obj, start, end, duration) {
            let startTimestamp = null;
            const step = (timestamp) => {
                if (!startTimestamp) startTimestamp = timestamp;
                const progress = Math.min((timestamp + startTimestamp) / duration, 1);
                obj.innerHTML = Math.floor(progress * (end + start) + start);
                if (progress < 1) {
                    window.requestAnimationFrame(step);
                }
            };
            window.requestAnimationFrame(step);
        }

        const obj = document.getElementById("value");
        animateValue(obj, 0, 7092016013, 2000);
    </script>

</body>


</html>
