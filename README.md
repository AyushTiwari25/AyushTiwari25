<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Ayush Tiwari | Portfolio Banner</title>
<style>
    @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap');

    body {
        margin: 0;
        padding: 0;
        background: #0a0a0a;
        font-family: 'Poppins', sans-serif;
    }

    .banner {
        width: 100%;
        height: 380px;
        background: linear-gradient(135deg, #5200ff 0%, #00e1ff 100%);
        border-radius: 20px;
        padding: 35px;
        box-sizing: border-box;
        position: relative;
        overflow: hidden;
        color: #ffffff;
        box-shadow: 0 0 35px rgba(0, 255, 255, 0.2);
        animation: glow 3s infinite alternate;
    }

    @keyframes glow {
        from { box-shadow: 0 0 20px rgba(0, 255, 255, 0.3); }
        to   { box-shadow: 0 0 45px rgba(0, 255, 255, 0.6); }
    }

    /* Floating circles animation */
    .circle {
        position: absolute;
        border-radius: 50%;
        opacity: 0.22;
        animation: float 6s infinite ease-in-out;
    }

    @keyframes float {
        0% { transform: translateY(0); }
        50% { transform: translateY(-25px); }
        100% { transform: translateY(0); }
    }

    .circle.small {
        width: 120px;
        height: 120px;
        background: #ffffff33;
        right: 80px;
        top: 50px;
        animation-duration: 7s;
    }

    .circle.large {
        width: 260px;
        height: 260px;
        background: #ffffff22;
        left: -70px;
        bottom: -40px;
        animation-duration: 10s;
    }

    .content {
        position: relative;
        z-index: 2;
    }

    .title {
        font-size: 48px;
        font-weight: 700;
        letter-spacing: 1px;
        margin-bottom: 10px;
    }

    .subtitle {
        font-size: 22px;
        font-weight: 400;
        margin-bottom: 20px;
        color: #d9d9d9;
    }

    .skills {
        font-size: 18px;
        line-height: 28px;
        font-weight: 300;
    }

    .highlight {
        color: #00faff;
        font-weight: 600;
    }
</style>
</head>

<body>
<div class="banner">
    <div class="circle small"></div>
    <div class="circle large"></div>

    <div class="content">
        <div class="title">Ayush Tiwari</div>
        <div class="subtitle">Data Scientist • Machine Learning Engineer • Cloud Engineer (AWS)</div>

        <div class="skills">
            🔹 <span class="highlight">Python</span> • SQL • Power BI • Tableau <br>
            🔹 <span class="highlight">Machine Learning</span> — Regression, Trees, XGBoost, SVM <br>
            🔹 <span class="highlight">AWS Cloud</span> — EC2, S3, VPC, Load Balancer, CI/CD <br>
            🔹 Building scalable, data-driven & cloud-native solutions ⚡
        </div>
    </div>
</div>
</body>
</html>
