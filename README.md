## EventCity
* Este é um sistema de eventos e cidades com uma relação N-1 entre eles:
  - Neste sistema, somente as rotas de leitura (GET) de eventos e cidades são públicas (não precisa de login).
  - Usuários CLIENT podem também inserir (POST) novos eventos. Os demais acessos são permitidos apenas a usuários ADMIN.
  
* Regras de autorização do ResourceServerConfig descritas em linguagem natural.
  - Os endpoints de login e do H2 devem ser públicos
  - Os endpoints GET para /cities e /events devem ser públicos
  - O endpoint POST de /events deve requerer login de ADMIN ou CLIENT
  - Todos demais endpoints devem requerer login de ADMIN
