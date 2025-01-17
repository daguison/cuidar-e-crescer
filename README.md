<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mini Curso - Planejamento de Rotina do Bebê</title>
    <style>
        /* Estilo básico para as abas */
        .tabs {
            display: flex;
            cursor: pointer;
            margin-bottom: 20px;
        }
        .tabs div {
            padding: 10px;
            background-color: #f0f0f0;
            margin-right: 5px;
            border-radius: 5px;
        }
        .tabs div:hover {
            background-color: #e0e0e0;
        }
        .content {
            display: none;
        }
        .active {
            display: block;
        }
        .tab-content {
            padding: 15px;
            background-color: #fafafa;
            border-radius: 5px;
        }
        /* Estilos adicionais */
        body {
            font-family: Arial, sans-serif;
            padding: 20px;
        }
    </style>
</head>
<body>

    <h1>Mini Curso: Planejamento de Rotina do Bebê</h1>
    <p>Bem-vindo ao mini curso! Escolha o dia para acessar os conteúdos.</p>
    
    <div class="tabs">
        <div onclick="showContent(1)">Dia 1: Necessidades do Bebê</div>
        <div onclick="showContent(2)">Dia 2: Alimentação Planejada</div>
        <div onclick="showContent(3)">Dia 3: Rotina de Sono</div>
        <div onclick="showContent(4)">Dia 4: Rotina Familiar</div>
        <div onclick="showContent(5)">Dia 5: Ajustando a Rotina</div>
    </div>

    <!-- Conteúdo para o Dia 1 -->
    <div id="day1" class="content tab-content">
        <h3>Dia 1: Entenda as Necessidades do Seu Bebê</h3>
        <p>Conteúdo do Dia 1...</p>
        <a href="link_para_o_material_dia1.pdf" download>Baixar material complementar</a>
    </div>

    <!-- Conteúdo para o Dia 2 -->
    <div id="day2" class="content tab-content">
        <h3>Dia 2: Montando um Horário de Alimentação</h3>
        <p>Conteúdo do Dia 2...</p>
        <a href="link_para_o_material_dia2.pdf" download>Baixar material complementar</a>
    </div>

    <!-- Conteúdo para o Dia 3 -->
    <div id="day3" class="content tab-content">
        <h3>Dia 3: Garantindo um Sono Tranquilo</h3>
        <p>Conteúdo do Dia 3...</p>
        <a href="link_para_o_material_dia3.pdf" download>Baixar material complementar</a>
    </div>

    <!-- Conteúdo para o Dia 4 -->
    <div id="day4" class="content tab-content">
        <h3>Dia 4: Planejamento Familiar</h3>
        <p>Conteúdo do Dia 4...</p>
        <a href="link_para_o_material_dia4.pdf" download>Baixar material complementar</a>
    </div>

    <!-- Conteúdo para o Dia 5 -->
    <div id="day5" class="content tab-content">
        <h3>Dia 5: Ajustando a Rotina da Família</h3>
        <p>Conteúdo do Dia 5...</p>
        <a href="link_para_o_material_dia5.pdf" download>Baixar material complementar</a>
    </div>

    <script>
        // Função para mostrar o conteúdo da aba selecionada
        function showContent(day) {
            // Esconde todos os conteúdos
            let contents = document.querySelectorAll('.content');
            contents.forEach(function(content) {
                content.classList.remove('active');
            });

            // Mostra o conteúdo correspondente
            document.getElementById('day' + day).classList.add('active');
        }

        // Exibe o conteúdo do Dia 1 por padrão
        showContent(1);
    </script>

</body>
</html>
