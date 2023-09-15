# Atividade1509
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>panda</title>
</head>
<body>
    <style>
    table
    {
        margin-left: auto;
        margin-right: auto;
        margin-top: 80px;
        background-color: #f5c0ff;
        border-radius: 10pt;
    }
    .td
    {
        width: 100px;
        height: 60px;
        border-style: groove;
        border-radius: 8pt;
        text-align: center;
        font-family: Arial, Helvetica, sans-serif;
        font-size: 30px;
        border-width: 2px;
        border-color: black;
        background-color: azure;
    }
    #mes
    {
        margin-left: auto;
        margin-right: auto;
        margin-top: 50px;
        height: 100px;
        width: 1000px;
        text-align: center;
        font-size: 45px;
        font-family: cursive;
    }
    #dom
    {
        background-color: rgb(255, 0, 170);
    }
    .title
    {
        font-size: 80px;
        font-family: cursive;
        text-align: center;
        margin-left: auto;
        margin-right: auto;
        margin-top: 60px;
        width: 800px;
        height: 80px;
    }
    .anulartd
    {
        border-style: none;
    }
    #dias
    {
        background-color: rgb(136, 0, 255);
    }
    body
    {
        background-color: rgb(194, 51, 255);
    }

    
    
    
    </style>
    <script lang="javascript">
    var umaData, ano, mes, d, lastday, c;

    ano = parseInt(window.prompt("digite um ano, por favor "));
    mes = parseInt(window.prompt("Digite seu mês, por favor "));

    umaData = new Date();
    umaData.setDate(1);
    umaData.setMonth(mes-1);
    umaData.setFullYear(ano);

    switch (mes)
    {
        case 1: document.write("<div class='title'>Janeiro de"  + ano + "</div>") ; break; 
        case 2: document.write("<div class='title'>Fevereiro de " + ano + "</div>"); break;
        case 3: document.write("<div class='title'>Março de " + ano + "</div>"); break;
        case 4: document.write("<div class='title'>Abril de " + ano + "</div>"); break;
        case 5: document.write("<div class='title'>Maio de " + ano + "</div>"); break;
        case 6: document.write("<div class='title'>Junho de " + ano + "</div>"); break;
        case 7: document.write("<div class='title'>Julho de " + ano + "</div>"); break;
        case 8: document.write("<div class='title'>Agosto de " + ano + "</div>"); break;
        case 9: document.write("<div class='title'>Setembro de " + ano + "</div>"); break;
        case 10: document.write("<div class='title'>Outubro de " + ano + "</div>"); break;
        case 11: document.write("<div class='title'>Novembro de " + ano + "</div>"); break;
        case 12: document.write("<div class='title'>Dezembro de " + ano + "</div>"); break;
    }

    document.write("<table border=3>");
    document.write("<tr><td id='dom' class='td'>DOM</td><td class='td' id='dias'>SEG</td><td class='td' id='dias'>TER</td><td class='td' id='dias'>QUA</td><td class='td' id='dias'>QUI</td><td class='td' id='dias'>SEX</td><td class='td' id='dias'>SÁB</td></tr>");

    switch (umaData.getDay())
        {
            case 0: c = 0; break;
            case 1: document.write("<tr> <td></td>"); c = 1; break;
            case 2: document.write("<tr> <td colspan='2' class='anulartd'></td>"); c = 2; break;
            case 3: document.write("<tr> <td colspan='3' class='anulartd'></td>"); c = 3; break;
            case 4: document.write("<tr> <td colspan='4' class='anulartd'></td>"); c = 4; break;
            case 5: document.write("<tr> <td colspan='5' class='anulartd'></td>"); c = 5; break;
            case 6: document.write("<tr> <td colspan='6' class='anulartd'></td>"); c = 6; break;
        }

    if ((ano % 4 == 0) && (mes == 2))
    {
        lastday = 29;
    }else if (mes == 2)
        {
            lastday = 28;
        }else if (mes == 1 || 3 || 5 || 7 || 8 || 10 || 12)
            {
                lastday = 31;
            }else
                {
                    lastday = 30;
                }

    
    for(d = 1; d <= lastday; d++)
    {
        c++;

        if (c == 0)
        {
            document.write("<tr>");
        }
        
        if (c == 1)
        {
            document.write("<td class='td' id='dom'>" + d + "</td>");
        }else
            {
                document.write("<td class='td'>" + d + "</td>");
            }
        
        if (c == 7)
        {
            document.write("</tr>")
            c = 0;
        }
        
        

    }
    </script>
</body>
</html><!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>panda</title>
</head>
<body>
    <style>
    table
    {
        margin-left: auto;
        margin-right: auto;
        margin-top: 80px;
        background-color: #f5c0ff;
        border-radius: 10pt;
    }
    .td
    {
        width: 100px;
        height: 60px;
        border-style: groove;
        border-radius: 8pt;
        text-align: center;
        font-family: Arial, Helvetica, sans-serif;
        font-size: 30px;
        border-width: 2px;
        border-color: black;
        background-color: azure;
    }
    #mes
    {
        margin-left: auto;
        margin-right: auto;
        margin-top: 50px;
        height: 100px;
        width: 1000px;
        text-align: center;
        font-size: 45px;
        font-family: cursive;
    }
    #dom
    {
        background-color: rgb(255, 0, 170);
    }
    .title
    {
        font-size: 80px;
        font-family: cursive;
        text-align: center;
        margin-left: auto;
        margin-right: auto;
        margin-top: 60px;
        width: 800px;
        height: 80px;
    }
    .anulartd
    {
        border-style: none;
    }
    #dias
    {
        background-color: rgb(136, 0, 255);
    }
    body
    {
        background-color: rgb(194, 51, 255);
    }

    
    
    
    </style>
    <script lang="javascript">
    var umaData, ano, mes, d, lastday, c;

    ano = parseInt(window.prompt("digite um ano, por favor "));
    mes = parseInt(window.prompt("Digite seu mês, por favor "));

    umaData = new Date();
    umaData.setDate(1);
    umaData.setMonth(mes-1);
    umaData.setFullYear(ano);

    switch (mes)
    {
        case 1: document.write("<div class='title'>Janeiro de"  + ano + "</div>") ; break; 
        case 2: document.write("<div class='title'>Fevereiro de " + ano + "</div>"); break;
        case 3: document.write("<div class='title'>Março de " + ano + "</div>"); break;
        case 4: document.write("<div class='title'>Abril de " + ano + "</div>"); break;
        case 5: document.write("<div class='title'>Maio de " + ano + "</div>"); break;
        case 6: document.write("<div class='title'>Junho de " + ano + "</div>"); break;
        case 7: document.write("<div class='title'>Julho de " + ano + "</div>"); break;
        case 8: document.write("<div class='title'>Agosto de " + ano + "</div>"); break;
        case 9: document.write("<div class='title'>Setembro de " + ano + "</div>"); break;
        case 10: document.write("<div class='title'>Outubro de " + ano + "</div>"); break;
        case 11: document.write("<div class='title'>Novembro de " + ano + "</div>"); break;
        case 12: document.write("<div class='title'>Dezembro de " + ano + "</div>"); break;
    }

    document.write("<table border=3>");
    document.write("<tr><td id='dom' class='td'>DOM</td><td class='td' id='dias'>SEG</td><td class='td' id='dias'>TER</td><td class='td' id='dias'>QUA</td><td class='td' id='dias'>QUI</td><td class='td' id='dias'>SEX</td><td class='td' id='dias'>SÁB</td></tr>");

    switch (umaData.getDay())
        {
            case 0: c = 0; break;
            case 1: document.write("<tr> <td></td>"); c = 1; break;
            case 2: document.write("<tr> <td colspan='2' class='anulartd'></td>"); c = 2; break;
            case 3: document.write("<tr> <td colspan='3' class='anulartd'></td>"); c = 3; break;
            case 4: document.write("<tr> <td colspan='4' class='anulartd'></td>"); c = 4; break;
            case 5: document.write("<tr> <td colspan='5' class='anulartd'></td>"); c = 5; break;
            case 6: document.write("<tr> <td colspan='6' class='anulartd'></td>"); c = 6; break;
        }

    if ((ano % 4 == 0) && (mes == 2))
    {
        lastday = 29;
    }else if (mes == 2)
        {
            lastday = 28;
        }else if (mes == 1 || 3 || 5 || 7 || 8 || 10 || 12)
            {
                lastday = 31;
            }else
                {
                    lastday = 30;
                }

    
    for(d = 1; d <= lastday; d++)
    {
        c++;

        if (c == 0)
        {
            document.write("<tr>");
        }
        
        if (c == 1)
        {
            document.write("<td class='td' id='dom'>" + d + "</td>");
        }else
            {
                document.write("<td class='td'>" + d + "</td>");
            }
        
        if (c == 7)
        {
            document.write("</tr>")
            c = 0;
        }
        
        

    }
    </script>
</body>
</html>
