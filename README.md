# NutricaoEscaleira
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Planos - Nutrição Esportiva e Clínica</title>

    <!-- Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@300;400;600;700;800&display=swap" rel="stylesheet">
    <style>
        /* RESET e ESTILO GERAL */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Montserrat', sans-serif;
            background: linear-gradient(135deg, #2ecc71, #27ae60);
            padding: 30px;
            color: #2d3436;
            line-height: 1.6;
        }

        .container {
            max-width: 1100px;
            margin: 0 auto;
            background: #fff;
            border-radius: 20px;
            overflow: hidden;
            box-shadow: 0 25px 50px rgba(0, 0, 0, 0.15);
        }

        header {
            background: linear-gradient(135deg, #27ae60, #2ecc71);
            color: #fff;
            padding: 60px 20px;
            text-align: center;
            border-bottom: 2px solid #fff;
        }

        header h1 {
            font-size: 42px;
            font-weight: 700;
            letter-spacing: 1px;
        }

        header p {
            font-size: 18px;
            opacity: 0.9;
        }

        section {
            padding: 50px 30px;
        }

        .section-title {
            text-align: center;
            font-size: 32px;
            font-weight: 700;
            color: #2d3436;
            margin-bottom: 40px;
        }

        .table {
            width: 100%;
            border-collapse: collapse;
            margin-bottom: 40px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
        }

        .table th {
            background: #2ecc71;
            color: #fff;
            padding: 15px;
        }

        .table td {
            padding: 14px;
            border-bottom: 1px solid #eee;
            text-align: center;
        }

        .highlight {
            background: #f1fff5;
            font-weight: 700;
            color: #27ae60;
        }

        .plan-card {
            background: #f8f9fa;
            padding: 30px;
            border-radius: 15px;
            margin-bottom: 30px;
            box-shadow: 0 5px 20px rgba(0, 0, 0, 0.05);
            transition: transform 0.3s, box-shadow 0.3s;
        }

        .plan-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
        }

        .plan-card h3 {
            margin-bottom: 15px;
            font-size: 22px;
            color: #27ae60;
        }

        .banner {
            background: linear-gradient(135deg, #2ecc71, #27ae60);
            color: white;
            padding: 40px;
            text-align: center;
            border-radius: 15px;
            margin-top: 30px;
        }

        .banner h2 {
            font-size: 28px;
            margin-bottom: 20px;
        }

        .cta {
            text-align: center;
            margin: 40px 0;
        }

        .btn {
            display: inline-block;
            background: #25D366;
            color: white;
            padding: 18px 40px;
            border-radius: 40px;
            font-weight: 700;
            text-decoration: none;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .btn:hover {
            transform: scale(1.05);
            box-shadow: 0 8px 20px rgba(37, 211, 102, 0.3);
        }

        footer {
            background: #2d3436;
            color: white;
            text-align: center;
            padding: 30px;
            margin-top: 50px;
        }

        /* Responsividade */
        @media (max-width: 768px) {
            .section-title {
                font-size: 28px;
            }

            header h1 {
                font-size: 30px;
            }

            .table th,
            .table td {
                font-size: 13px;
                padding: 10px;
            }

            .plan-card {
                padding: 20px;
            }

            .banner h2 {
                font-size: 24px;
            }

            .cta {
                margin: 30px 0;
            }

            .btn {
                padding: 16px 35px;
                font-size: 16px;
            }
        }

        @media (max-width: 480px) {
            .container {
                padding: 10px;
            }

            header {
                padding: 40px 20px;
            }

            .btn {
                font-size: 14px;
            }
        }
    </style>
</head>

<body>

<div class="container">

    <header>
        <h1>📊 Planos de Longo Prazo</h1>
        <p>Quanto mais ciclos, maior seu desconto!</p>
    </header>

    <section>
        <h2 class="section-title">PACOTES PRESENCIAIS (avulso R$250)</h2>

        <table class="table">
            <thead>
                <tr>
                    <th>Pacote</th>
                    <th>Duração</th>
                    <th>Valor</th>
                    <th>Economia</th>
                    <th>Desconto</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td>2 ciclos</td>
                    <td>3 meses</td>
                    <td class="highlight">R$ 440</td>
                    <td>R$ 60</td>
                    <td>12%</td>
                </tr>
                <tr>
                    <td>4 ciclos</td>
                    <td>6 meses</td>
                    <td class="highlight">R$ 840</td>
                    <td>R$ 160</td>
                    <td>16%</td>
                </tr>
                <tr>
                    <td>8 ciclos</td>
                    <td>12 meses</td>
                    <td class="highlight">R$ 1.520</td>
                    <td>R$ 480</td>
                    <td>24%</td>
                </tr>
            </tbody>
        </table>

        <h2 class="section-title">PACOTES ONLINE (avulso R$220)</h2>

        <table class="table">
            <thead>
                <tr>
                    <th>Pacote</th>
                    <th>Duração</th>
                    <th>Valor</th>
                    <th>Economia</th>
                    <th>Desconto</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td>2 ciclos</td>
                    <td>3 meses</td>
                    <td class="highlight">R$ 390</td>
                    <td>R$ 50</td>
                    <td>11%</td>
                </tr>
                <tr>
                    <td>4 ciclos</td>
                    <td>6 meses</td>
                    <td class="highlight">R$ 740</td>
                    <td>R$ 140</td>
                    <td>16%</td>
                </tr>
                <tr>
                    <td>8 ciclos</td>
                    <td>12 meses</td>
                    <td class="highlight">R$ 1.340</td>
                    <td>R$ 420</td>
                    <td>24%</td>
                </tr>
            </tbody>
        </table>
    </section>

    <section>
        <h2 class="section-title">🏆 Planos Especializados</h2>

        <div class="plan-card">
            <h3>Plano Atleta</h3>
            <p>Consulta a cada 6 semanas + ajustes via WhatsApp</p>
            <p><
