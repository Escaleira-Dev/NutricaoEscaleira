# NutricaoEscaleira
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Nutrição Esportiva & Clínica para resultados reais com acompanhamento personalizado. Atendimentos clínicos e esportivos com foco em saúde e performance.">
    <meta name="author" content="Helio Escaleira">
    <title>Folder - Nutrição Esportiva e Clínica</title>
    <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Montserrat:wght@300;400;600;700;800&family=Playfair+Display:wght@700&display=swap">
    <style>
        /* RESET e ESTILO GERAL */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Montserrat', sans-serif;
            background: linear-gradient(135deg, #2ecc71 0%, #27ae60 100%);
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            padding: 20px;
        }

        .folder-container {
            width: 100%;
            max-width: 800px;
            background: white;
            border-radius: 20px;
            overflow: hidden;
            box-shadow: 0 25px 50px -12px rgba(0, 0, 0, 0.5);
        }

        /* CAPA COM LOGO DE FUNDO */
        .cover {
            background: linear-gradient(135deg, rgba(46,204,113,0.95) 0%, rgba(39,174,96,0.95) 50%, rgba(52,152,219,0.95) 100%);
            padding: 100px 40px;
            text-align: center;
            position: relative;
            overflow: hidden;
        }

        .cover::before {
            content: '';
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            width: 80%;
            height: 80%;
            background: url('path_to_logo.png') center/contain no-repeat;
            opacity: 0.25;
            filter: blur(2px);
        }

        .cover-content {
            position: relative;
            z-index: 2;
        }

        .cover h1 {
            font-family: 'Playfair Display', serif;
            font-size: 56px;
            color: white;
            margin-bottom: 15px;
            text-shadow: 3px 3px 8px rgba(0, 0, 0, 0.4);
            font-weight: 700;
            letter-spacing: 1px;
        }

        .cover .subtitle {
            font-size: 24px;
            color: rgba(255, 255, 255, 0.95);
            font-weight: 300;
            letter-spacing: 5px;
            text-transform: uppercase;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.3);
        }

        /* CONTEÚDO INTERNO */
        .content {
            padding: 50px 40px;
            background: linear-gradient(to bottom, #ffffff 0%, #f8f9fa 100%);
            position: relative;
        }

        /* BANNER DESTAQUE */
        .highlight-banner {
            background: linear-gradient(135deg, #2ecc71 0%, #27ae60 100%);
            color: white;
            padding: 40px;
            border-radius: 15px;
            margin: 20px 0 40px;
            text-align: center;
            position: relative;
            overflow: hidden;
        }

        .highlight-banner h3 {
            font-size: 28px;
            margin-bottom: 15px;
            font-weight: 700;
        }

        .highlight-banner p {
            font-size: 18px;
            max-width: 500px;
            margin: 0 auto;
            opacity: 0.95;
        }

        /* ATENDIMENTOS */
        .section {
            margin-bottom: 40px;
        }

        .section-title {
            font-family: 'Playfair Display', serif;
            font-size: 32px;
            color: #2d3436;
            margin-bottom: 25px;
            display: flex;
            align-items: center;
            gap: 15px;
            text-align: center;
            justify-content: center;
        }

        .services-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 25px;
            margin-top: 20px;
        }

        .service-box {
            background: white;
            border: 2px solid #e0e0e0;
            border-radius: 15px;
            padding: 35px 30px;
            text-align: center;
            transition: all 0.3s;
            position: relative;
            overflow: hidden;
        }

        .service-box:hover {
            border-color: #2ecc71;
            transform: scale(1.02);
            box-shadow: 0 10px 30px rgba(46, 204, 113, 0.2);
        }

        .service-box .service-icon {
            font-size: 55px;
            margin-bottom: 20px;
            display: block;
        }

        .service-box h3 {
            font-size: 24px;
            color: #2d3436;
            margin-bottom: 20px;
            font-weight: 700;
        }

        .service-box ul {
            list-style: none;
            text-align: left;
            font-size: 15px;
            color: #636e72;
            line-height: 1.9;
            padding-left: 10px;
        }

        .service-box ul li {
            margin-bottom: 10px;
            padding-left: 25px;
            position: relative;
        }

        .service-box ul li::before {
            content: '✓';
            position: absolute;
            left: 0;
            top: 0;
            color: #2ecc71;
            font-weight: bold;
            font-size: 18px;
        }

        /* DIFERENCIAIS */
        .differentials {
            background: linear-gradient(135deg, #2d3436 0%, #1a1a2e 100%);
            color: white;
            padding: 40px;
            border-radius: 15px;
            margin: 40px 0;
            text-align: center;
        }

        .differentials h3 {
            font-size: 28px;
            margin-bottom: 25px;
            font-family: 'Playfair Display', serif;
        }

        .differentials-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 20px;
        }

        /* COMO FUNCIONA */
        .how-it-works {
            display: flex;
            justify-content: space-around;
            flex-wrap: wrap;
            margin-top: 30px;
            text-align: center;
            gap: 20px;
        }

        .step {
            flex: 1;
            min-width: 140px;
            padding: 30px 20px;
            background: white;
            border-radius: 15px;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.08);
            transition: transform 0.3s;
            border-top: 4px solid #2ecc71;
        }

        .step:hover {
            transform: translateY(-5px);
        }

        .step .step-icon {
            font-size: 45px;
            margin-bottom: 15px;
            display: block;
        }

        .step h4 {
            color: #2d3436;
            margin-bottom: 8px;
            font-size: 16px;
            font-weight: 700;
        }

        .step p {
            font-size: 13px;
            color: #636e72;
            line-height: 1.4;
        }

        /* CONTATO COM LOGO DE FUNDO */
        .contact-section {
            background: linear-gradient
