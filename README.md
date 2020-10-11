# CONTA-LETRAS-A
projeto faculdade
onEvent("button_contarletra_a", "click", function( ) {
  var palavra = "";
  var totalAs = 0;
  palavra = getText("text_input_palavra");
  console.log("Palavra digitada: " + palavra);
  for (var pos = 0; pos < palavra.length; pos++) {
    console.log("pos: " + pos);
    console.log(palavra.substring(pos, pos + 1));
    //O if abaixo verifica se a letra na posicao i em MAIUSCULO é igual a A
    if (palavra.substring(pos, pos + 1).toUpperCase() == "A") {
      totalAs ++;
    }
  }
  setText("label_Resultado", totalAs);
});
