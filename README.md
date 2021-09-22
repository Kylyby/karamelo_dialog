# karamelo_dialog
## Karamelo ajuda você a criar facilmente uma pergunta com opções no console python

Para utilizá-lo, você deve primeiramente instalar uma dependência com o sequinte comando no terminal/shell:

pip3 install curtsies

agora digite os seguintes comandos no shell para instalar o Karamelo no replit


  git clone https://github.com/Kylyby/karamelo_dialog.git

  mv /home/runner/[pasta do projeto]/karamelo_dialog/karamelo.py /home/runner/[pasta do projeto]/
  
  rm -rf karamelo_dialog

  
no terceiro passo, [pasta do projeto] é o nome da pasta do seu projeto, se você tiver um projeto chamado "teste python", por exemplo, o nome da sua pasta será "teste-python" (sem as aspas)
  
### Como usar:
  
comece importando o arquivo:
  
  import karamelo
  
depois defina uma variável e nela chame a função:
  
  karamelorun = karamelo.dialog()
  
Dentro dela temos três parâmetros: Cor de fundo da seleção (bgcolor), número de opções que podem ser selecionadas (limit) e as opções (options)
  bgcolor deve ser uma string, limit uma int e options uma lista
  
  Exemplo:
  
  karamelorun = karamelo.dialog(bgcolor=red, limit=4, options=['um', 'dois', 'três', 'quatro'])
  
  cores aceitas noo bgcolor:
  'black'
  'red'
  'green'
  'yellow'
  'blue'
  'purple'
  'cyan'
  
no final, a varável definida acima vai retornal um valor, você pode utilizá-lo para definir o que cada opção faz. Ele sempre começa do zero, ou seja, o valor da opção vai ser a posição dela menos 1, por exemplo: a 3ª opção vai ter o valor de 2
  
exemplo do uso:
  
  if karamelorun == 0:
    print('abacaxi')
  elif karamelorun == 1:
    print('banana')
  elif karamelorun == 2:
    print('maçã')
  elif karamelorun == 3:
    print('uva')
  
No final desse exemplo ficamos com o seguinte código:
  
  karamelorun = karamelo.dialog(bgcolor=red, limit=4, options=['um', 'dois', 'três', 'quatro'])
  
  if karamelorun == 0:
    print('abacaxi')
  elif karamelorun == 1:
    print('banana')
  elif karamelorun == 2:
    print('maçã')
  elif karamelorun == 3:
    print('uva')
