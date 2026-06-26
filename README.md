<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Clubinho da Espuma</title>
<link rel="stylesheet" href="style.css">

</head>

<body>
<div class="container">

<div class="esquerda">

<h1>Clubinho da Espuma</h1>

<form id="formulario" class="formulario">

<div class="campo">
<label>Nome do Pet</label>
<input type="text" id="nome" required>
</div>

<div class="campo">
<label>Porte do Pet</label>

<select id="porte" required>

<option value="">Selecione</option>
<option>Pequeno</option>
<option>Médio</option>
<option>Grande</option>

</select>

</div>

<div class="campo">
<label>Raça do Pet</label>
<input type="text" id="raca" required>
</div>

<div class="campo">
<label>Horário desejado</label>

<select id="horario" required>

<option value="">Selecione</option>

<option>09:00</option>
<option>10:00</option>
<option>11:00</option>
<option>13:00</option>
<option>14:00</option>
<option>15:00</option>
<option>16:00</option>
<option>17:00</option>

</select>

</div>

<div class="campo">

<label>Telefone para contato</label>
<input type="tel" id="telefone" required>

</div>

<div class="botao">

<button type="submit">Agendar</button>

</div>

</form>

</div>

<div class="direita">

<img src="img/clubinho da espuma.jpeg" alt="Logo Clubinho da Espuma">

</div>

</div>

<script>

document.getElementById("formulario").addEventListener("submit",function(e){

e.preventDefault();

let nome=document.getElementById("nome").value;
let porte=document.getElementById("porte").value;
let raca=document.getElementById("raca").value;
let horario=document.getElementById("horario").value;
let telefone=document.getElementById("telefone").value;

let numero="5511999999999";

let mensagem=`Olá!

Gostaria de agendar um banho.

🐶 Nome do Pet: ${nome}
🐾 Raça: ${raca}
📏 Porte: ${porte}
🕐 Horário: ${horario}
📱 Telefone: ${telefone}`;

window.open(`https://wa.me/${seu telefone}?text=${encodeURIComponent(mensagem)}`,"_blank");

});

    </script>
</body>
</html>
