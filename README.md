<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Amüre W. Anat</title>
    <link href="https://fonts.googleapis.com/css2?family=Questrial&display=swap" rel="stylesheet">
    <style>
        :root {
            --dark-blue: #0f1b2d;
            --steel-blue: #2e4a6b;
            --light-gray: #f8f9fa;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Questrial', sans-serif;
        }

        body {
            background-color: var(--light-gray);
            color: var(--dark-blue);
            line-height: 1.6;
            min-height: 100vh;
        }

        .container {
            display: flex;
            flex-wrap: wrap;
            height: 100vh;
            padding: 40px;
            gap: 40px;
        }

        .author-portrait {
            flex: 1;
            background-image: url('your-image.jpg');
            background-size: cover;
            background-position: center;
            border-radius: 8px;
            box-shadow: 8px 8px 0px var(--steel-blue);
            min-height: 300px;
        }

        .text-content {
            flex: 1;
            display: flex;
            flex-direction: column;
            justify-content: center;
            padding-right: 15%;
        }

        .salutation {
            font-size: 46px;
            margin-bottom: 30px;
            letter-spacing: -1.5px;
        }

        .main-text {
            font-size: 16px;
            max-width: 500px;
            line-height: 1.8;
        }

        .decorative-line {
            width: 100px;
            height: 3px;
            background: var(--steel-blue);
            margin: 30px 0;
        }

        .section {
            margin-top: 60px;
        }

        .section-title {
            font-size: 32px;
            margin-bottom: 15px;
            color: var(--steel-blue);
        }

        @media (max-width: 768px) {
            .container {
                flex-direction: column;
                align-items: center;
                padding: 20px;
                height: auto;
            }
            .text-content {
                padding-right: 0;
                text-align: center;
            }
            .salutation {
                font-size: 36px;
            }
            .main-text {
                max-width: 100%;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="author-portrait"></div>
        
        <div class="text-content">
            <div class="salutation">Dear,</div>
            <div class="decorative-line"></div>
            <p class="main-text">
                Here we are. You and me on a digital layer. Face to face, in different times, in different places. Check my debut novel, read it through, pay attention, drop the book and forget you even read it. Because nothing is too serious, but the tyranny of the rich, and drudgery of the dull.
            </p>
        </div>
    </div>

    <div class="container section">
        <div class="text-content">
            <div class="section-title">Bio</div>
            <p class="main-text">
                Amüre W. Anat is a writer, thinker, and observer of the human condition. Their work delves into the intricacies of existence, the absurdity of power, and the poetry of the mundane.
            </p>
        </div>
    </div>

    <div class="container section">
        <div class="text-content">
            <div class="section-title">Dear God, King David is Dead</div>
            <p class="main-text">
                The echoes of a fallen king reverberate through time. His reign, his legacy, his name—erased by the tide of forgetfulness. But in the void he left behind, who will rise?
            </p>
        </div>
    </div>
</body>
</html>
