# festival

Descreva aqui as alterações/correções que fez

## 1
- adicionei ".order_by("data")" em views.py para ordenar pela data.

## 2 
- a linha "ordering = ["dia__data", "hora"]" ordena os palcos pelo dia e depois pela hora.

## 3
- O formulário ConcertoForm foi alterado para incluir todos os campos do modelo (banda, dia, hora, palco), permitindo a edição completa de um concerto.
- O template editar_concerto.html foi corrigido para apresentar informação do concerto

## 4
- Foi criada a rota concertos/<int:concerto_id>/apagar/
- Foi implementada a view apagar_concerto_view
- Foi adicionado o botão "Apagar concerto" no template concerto.html

## 5
- Criei a rota concertos/criar/
- Implementei a view criar_concerto_view
- Criei template criar_concerto.html
- Coloquei o link certo para o "criar_concerto.html" no layout.html

## 6
- O símbolo ♿ foi adicionado inline no <h2>
- Foi usada uma condição {% if %} para o mostrar apenas quando aplicável

## 7
- Criada a view editar_palco_view com ModelForm e instance=palco
- Adicionada a rota palcos/<int:palco_id>/editar/
- Criado template editar_palco.html
- Ligado o botão “Editar palco” ao sistema de edição