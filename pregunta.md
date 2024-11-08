# Pregunta para el parcial

**¿Cuál de las siguientes prácticas es efectiva para prevenir ataques de inyección?**

<form id="quizForm">
  <input type="radio" name="answer" value="a" id="optionA">
  <label for="optionA">a) Evitar el uso de bases de datos.</label><br>
  
  <input type="radio" name="answer" value="b" id="optionB">
  <label for="optionB">b) Saneamiento de entradas de usuario.</label><br>
  
  <input type="radio" name="answer" value="c" id="optionC">
  <label for="optionC">c) Utilizar contraseñas largas.</label><br>
  
  <input type="radio" name="answer" value="d" id="optionD">
  <label for="optionD">d) Incluir muchos comentarios en el código.</label><br><br>
  
  <button type="button" onclick="checkAnswer()">Verificar respuesta</button>
</form>

<p id="result"></p>

<script>
function checkAnswer() {
  const selectedAnswer = document.querySelector('input[name="answer"]:checked');
  const result = document.getElementById("result");

  if (!selectedAnswer) {
    result.textContent = "Por favor, selecciona una respuesta.";
    result.style.color = "orange";
    return;
  }

  if (selectedAnswer.value === "b") {
    result.textContent = "¡Correcto! Saneamiento de entradas de usuario es una práctica efectiva para prevenir ataques de inyección.";
    result.style.color = "green";
  } else {
    result.textContent = "Incorrecto. La respuesta correcta es 'b) Saneamiento de entradas de usuario'.";
    result.style.color = "red";
  }
}
</script>


</body>
</html>

