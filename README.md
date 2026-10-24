# Central — atualizações

Canal de atualização do **Central**, um app pessoal para controlar o PC e a casa pelo celular
(agente no Windows + app Android).

Aqui ficam só os **pacotes de atualização** (em *Releases*). O agente instalado no PC confere este
canal a cada 6 horas e se atualiza sozinho.

## Segurança

- Cada pacote é **assinado** (Ed25519) com uma chave que só existe no PC de quem publica.
  O agente só instala se a assinatura conferir com a chave pública que vem dentro dele: um arquivo
  trocado aqui seria recusado.
- O manifesto (`atualizacao.json`) traz a versão, o SHA-256 do pacote e a assinatura.
- Os pacotes não têm token, senha, histórico nem dados de ninguém: cada instalação gera os seus.
