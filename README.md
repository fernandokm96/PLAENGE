<!DOCTYPE html>
<html>
<head>
    <title>Relatório de Desempenho Mensal - Campanha ALTO DO LINDOIA RESORT</title>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script> 
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 20px;
            background-color: #f4f4f4;
            color: #333;
            box-sizing: border-box;
        }
        .container {
            max-width: 1000px;
            margin: auto;
            background: #fff;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 2px 4px rgba(0,0,0,0.1);
        }
        h1, h2 {
            color: #0056b3;
            text-align: center;
            margin-bottom: 10px;
        }
        .date-info {
            text-align: center;
            color: #555;
            margin-bottom: 20px;
            font-size: 0.9em;
        }
        .summary-metrics {
            display: flex;
            justify-content: space-around;
            flex-wrap: wrap;
            gap: 20px;
            margin-bottom: 40px;
            text-align: center;
        }
        .metric-box {
            background-color: #e0f7fa;
            border-left: 5px solid #00bcd4;
            padding: 15px 20px;
            border-radius: 5px;
            flex: 1;
            min-width: 200px;
            box-shadow: 0 1px 3px rgba(0,0,0,0.1);
            box-sizing: border-box;
        }
        .metric-box h3 {
            margin: 0 0 5px 0;
            color: #007bff;
            font-size: 1.1em;
        }
        .metric-box p {
            margin: 0;
            font-size: 1.6em;
            font-weight: bold;
            color: #333;
        }
        .chart-container {
            width: 100%;
            height: 350px; /* Altura padrão para desktop */
            position: relative;
            margin-bottom: 40px;
            box-sizing: border-box;
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: 5px;
            background-color: #fff;
        }
        .chart-container canvas {
            max-width: 100% !important; 
            height: 100% !important;   
            display: block;
            opacity: 1;
            /* Opcional: para debug, para ver se o canvas está presente */
            /* border: 1px dashed red; */ 
        }

        .table-responsive {
            overflow-x: auto;
            margin-bottom: 30px;
        }
        table {
            width: 100%;
            border-collapse: collapse;
            min-width: 600px;
        }
        table, th, td {
            border: 1px solid #ddd;
        }
        th, td {
            padding: 12px;
            text-align: left;
            white-space: nowrap;
        }
        th {
            background-color: #0056b3;
            color: white;
        }
        tr:nth-child(even) {
            background-color: #f2f2f2;
        }
        .analysis {
            background-color: #e9f7ef;
            border-left: 5px solid #28a745;
            padding: 15px;
            margin-top: 30px;
            border-radius: 5px;
        }
        .analysis h3 {
            color: #28a745;
            margin-top: 0;
        }

        /* Responsive adjustments */
        @media (max-width: 768px) {
            body {
                padding: 10px;
            }
            .container {
                padding: 15px;
            }
            .summary-metrics .metric-box {
                flex-basis: 48%;
                min-width: unset;
            }
            h1 {
                font-size: 1.8em;
            }
            h2 {
                font-size: 1.5em;
            }
            th, td {
                padding: 8px;
                font-size: 0.9em;
            }
            .chart-container {
                height: 300px; /* Ajusta a altura para tablets */
            }
        }

        @media (max-width: 480px) {
            .summary-metrics .metric-box {
                flex-basis: 100%;
            }
            h1 {
                font-size: 1.5em;
            }
            h2 {
                font-size: 1.3em;
            }
            .metric-box p {
                font-size: 1.4em;
            }
            .date-info {
                font-size: 0.8em;
            }
            .analysis ul {
                padding-left: 20px;
            }
            .chart-container {
                height: 250px; /* Ajusta a altura para celulares */
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Relatório de Desempenho Mensal - Campanha ALTO DO LINDOIA RESORT</h1>
        <p class="date-info">Período da Análise: Dezembro/2024 a Junho/2025</p>

        <h2>Principais Métricas da Campanha (Total)</h2>
        <div class="summary-metrics">
            <div class="metric-box">
                <h3>Total de Leads Gerados</h3>
                <p>450</p>
            </div>
            <div class="metric-box">
                <h3>Custo por Lead Médio</h3>
                <p>R$ 30,20</p>
            </div>
            <div class="metric-box">
                <h3>Valor Gasto Total</h3>
                <p>R$ 13.590,60</p>
            </div>
            <div class="metric-box">
                <h3>Alcance Total</h3>
                <p>119.981</p>
            </div>
            <div class="metric-box">
                <h3>Impressões Totais</h3>
                <p>327.952</p>
            </div>
        </div>

        <h2>Detalhamento do Desempenho por Mês</h2>
        <div class="table-responsive">
            <table>
                <thead>
                    <tr>
                        <th>Mês</th>
                        <th>Leads</th>
                        <th>Alcance</th>
                        <th>Impressões</th>
                        <th>Custo por Lead</th>
                        <th>Valor Gasto</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td>DEZEMBRO DE 2024</td>
                        <td>141</td>
                        <td>38088</td>
                        <td>117829</td>
                        <td>R$ 36,64</td>
                        <td>R$ 5.165,97</td>
                    </tr>
                    <tr>
                        <td>JANEIRO DE 2025</td>
                        <td>202</td>
                        <td>43252</td>
                        <td>137328</td>
                        <td>R$ 25,75</td>
                        <td>R$ 5.201,47</td>
                    </tr>
                    <tr>
                        <td>FEVEREIRO DE 2025</td>
                        <td>48</td>
                        <td>10641</td>
                        <td>25184</td>
                        <td>R$ 25,48</td>
                        <td>R$ 1.223,16</td>
                    </tr>
                    <tr>
                        <td>MARÇO DE 2025</td>
                        <td>0</td>
                        <td>0</td>
                        <td>0</td>
                        <td>R$ 0,00</td>
                        <td>R$ 0,00</td>
                    </tr>
                    <tr>
                        <td>ABRIL DE 2025</td>
                        <td>13</td>
                        <td>3284</td>
                        <td>6180</td>
                        <td>R$ 33,63</td>
                        <td>R$ 437,18</td>
                    </tr>
                    <tr>
                        <td>MAIO DE 2025</td>
                        <td>43</td>
                        <td>21924</td>
                        <td>38056</td>
                        <td>R$ 35,01</td>
                        <td>R$ 1.505,57</td>
                    </tr>
                    <tr>
                        <td>JUNHO DE 2025</td>
                        <td>3</td>
                        <td>2792</td>
                        <td>3375</td>
                        <td>R$ 19,08</td>
                        <td>R$ 57,25</td>
                    </tr>
                </tbody>
            </table>
        </div>

        <h2>Gráficos de Tendência Mensal</h2>

        <div class="chart-container">
            <h3>Leads Gerados por Mês</h3>
            <canvas id="leadsByMonthChart"></canvas>
        </div>

        <div class="chart-container">
            <h3>Custo por Lead (CPL) por Mês</h3>
            <canvas id="cplByMonthChart"></canvas>
        </div>

        <div class="chart-container">
            <h3>Valor Gasto e Leads por Mês</h3>
            <canvas id="valorLeadsByMonthChart"></canvas>
        </div>

        <div class="analysis">
            <h3>Análise do Desempenho da Campanha ALTO DO LINDOIA RESORT</h3>
            <p>A campanha "ALTO DO LINDOIA RESORT" mostra uma performance variada de Dezembro de 2024 a Junho de 2025.</p>
            <ul>
                <li>**Picos de Leads e Investimento:** Janeiro de 2025 se destacou com o maior número de leads (202) e um CPL eficiente de R$ 25,75. Dezembro de 2024 também teve um alto volume de leads (141).</li>
                <li>**Meses de Menor Eficiência:** Junho de 2025, embora com o menor CPL (R$ 19,08), registrou um número muito baixo de leads (3) e o menor valor gasto (R$ 57,25), o que pode indicar um período de pouca veiculação ou testes. Maio de 2025 teve um aumento em leads (43) e valor gasto (R$ 1.505,57) em comparação a Abril, mas com um CPL (R$ 35,01) mais alto que os meses iniciais.</li>
                <li>**Pausa na Campanha:** Março de 2025 registrou 0 leads, 0 alcance, 0 impressões e R$ 0,00 de valor gasto, sugerindo uma interrupção completa da campanha nesse mês.</li>
                <li>**Recuperação e Variações:** Após a pausa em Março, a campanha demonstrou uma recuperação modesta em Abril (13 leads) e Maio (43 leads). O CPL teve flutuações, sendo mais baixo em Fevereiro (R$ 25,48) e Junho (R$ 19,08), e mais alto em Dezembro (R$ 36,64) e Maio (R$ 35,01).</li>
                <li>**Total Geral:** No período analisado, a campanha gerou um total de 450 leads, com um custo médio por lead de R$ 30,20 e um valor gasto total de R$ 13.590,60.</li>
            </ul>
        </div>
    </div>

    <script>
        // Função principal para inicializar os gráficos
        function initializeCharts() {
            const meses = ['DEZEMBRO DE 2024', 'JANEIRO DE 2025', 'FEVEREIRO DE 2025', 'MARÇO DE 2025', 'ABRIL DE 2025', 'MAIO DE 2025', 'JUNHO DE 2025'];
            const leads = [141, 202, 48, 0, 13, 43, 3];
            const alcance = [38088, 43252, 10641, 0, 3284, 21924, 2792];
            const impressoes = [117829, 137328, 25184, 0, 6180, 38056, 3375];
            const custoPorLead = [36.64, 25.75, 25.48, 0.00, 33.63, 35.01, 19.08];
            const valorGasto = [5165.97, 5201.47, 1223.16, 0.00, 437.18, 1505.57, 57.25];

            let myCharts = {}; // Para armazenar as instâncias dos gráficos

            function createChart(chartId, type, labels, datasets, options) {
                const ctx = document.getElementById(chartId);
                if (ctx) {
                    // Destrói o gráfico existente se houver um antes de criar um novo
                    if (myCharts[chartId]) {
                        myCharts[chartId].destroy();
                    }
                    myCharts[chartId] = new Chart(ctx, {
                        type: type,
                        data: {
                            labels: labels,
                            datasets: datasets
                        },
                        options: options
                    });
                } else {
                    console.error('Elemento canvas com ID "' + chartId + '" não encontrado.');
                }
            }

            const commonChartOptions = {
                responsive: true,
                maintainAspectRatio: false,
                plugins: {
                    legend: {
                        display: true
                    },
                    tooltip: {
                        callbacks: {
                            label: function(context) {
                                if (context.dataset.label.includes('R$')) {
                                    return context.dataset.label + ': R$ ' + context.parsed.y.toFixed(2);
                                }
                                return context.dataset.label + ': ' + context.parsed.y.toLocaleString();
                            }
                        }
                    }
                }
            };

            createChart('leadsByMonthChart', 'line', meses, [{
                label: 'Leads Gerados (Quant.)',
                data: leads,
                borderColor: 'rgba(75, 192, 192, 1)',
                backgroundColor: 'rgba(75, 192, 192, 0.2)',
                fill: true,
                tension: 0.3
            }], {
                ...commonChartOptions,
                scales: {
                    y: {
                        beginAtZero: true,
                        title: { display: true, text: 'Número de Leads' },
                        ticks: { callback: function(value) { return value.toLocaleString(); } }
                    },
                    x: { title: { display: true, text: 'Mês' } }
                }
            });

            createChart('cplByMonthChart', 'line', meses, [{
                label: 'Custo por Lead (R$)',
                data: custoPorLead,
                borderColor: 'rgba(255, 99, 132, 1)',
                backgroundColor: 'rgba(255, 99, 132, 0.2)',
                fill: true,
                tension: 0.3
            }], {
                ...commonChartOptions,
                scales: {
                    y: {
                        beginAtZero: true,
                        title: { display: true, text: 'Custo por Lead (R$)' },
                        ticks: { callback: function(value) { return 'R$ ' + value.toFixed(2); } }
                    },
                    x: { title: { display: true, text: 'Mês' } }
                }
            });

            createChart('valorLeadsByMonthChart', 'bar', meses, [
            {
                type: 'line',
                label: 'Leads Gerados (Quant.)',
                data: leads,
                borderColor: 'rgba(75, 192, 192, 1)',
                backgroundColor: 'rgba(75, 192, 192, 0.2)',
                fill: false,
                tension: 0.3,
                yAxisID: 'y-leads'
            },
            {
                type: 'bar',
                label: 'Valor Gasto (R$)',
                data: valorGasto,
                backgroundColor: 'rgba(54, 162, 235, 0.6)',
                borderColor: 'rgba(54, 162, 235, 1)',
                borderWidth: 1,
                yAxisID: 'y-valor'
            }], {
                ...commonChartOptions,
                interaction: { mode: 'index', intersect: false },
                scales: {
                    'y-valor': {
                        type: 'linear',
                        position: 'left',
                        beginAtZero: true,
                        title: { display: true, text: 'Valor Gasto (R$)' },
                        ticks: { callback: function(value) { return 'R$ ' + value.toFixed(2); } }
                    },
                    'y-leads': {
                        type: 'linear',
                        position: 'right',
                        beginAtZero: true,
                        title: { display: true, text: 'Número de Leads' },
                        grid: { drawOnChartArea: false },
                        ticks: { callback: function(value) { return value.toLocaleString(); } }
                    }
                },
                x: { title: { display: true, text: 'Mês' } }
            });

            // Adiciona um listener para o evento de resize da janela
            window.addEventListener('resize', () => {
                for (let chartId in myCharts) {
                    if (myCharts[chartId]) {
                        myCharts[chartId].resize();
                    }
                }
            });
        }

        // Tenta inicializar os gráficos assim que o DOM estiver pronto
        document.addEventListener('DOMContentLoaded', initializeCharts);

        // Adiciona um atraso maior como fallback para WebViews teimosos
        // Se DOMContentLoaded não for suficiente, este setTimeout garante uma segunda tentativa
        setTimeout(initializeCharts, 2000); // 2 segundos de atraso
    </script>
</body>
</html>
