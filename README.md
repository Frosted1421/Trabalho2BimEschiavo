Introdução:
Hoje irei falar sobre o YggDrasil Network, por mais que o projeto se encontre em fase Alfa e relativamente longe de uma fase estável o mesmo ja se pode ser implementado para testes e é relativamente estavel

O que é?
YggDrasil é esquema de roteamento compacto projetado para redes mesh ou redes internet-likes (como intranets), predominantemente é um esquema de caminho mais curto, onde a rede tenta encontrar o caminho mais direto para o destino.
Diferente de outros esquemas de roteamente muito utilizados hoje em dia, yggdrasil é fortemente descentralizado, amplamente auto organizavel e em grande parte auto recuperavel, com a topologia de rede adaptavel, fornecendo roteabilidade total entre todos os participantes, todos os nós no YggDrasil com varios pares atuam como roteadores.

Como funciona?

Todos os nós são identificados por uma chave publica criptografica, e endereços ipv6 são gerados a partir deste chave
Isso permite que, todos as aplicações que usam ipv6 para serem operadas, se tornem compativeis com o yggdrasil e o endereço permanece a medida que o nó se move pela rede.


Problema da internet hoje em dia:
A internet hoje em dia é totalmente hierarquica e estruturada, não segue uma topologia bem definida, e falta desta topologia nos traz diversos problemas:
-Tabelas de roteamentes enormes e ineficientes
-Um computador não sabe onde esta localizado na internet em relação a qualquer outra coisa
-Dificil examniar por onde o pacote ira passar sem que antes o envie.

Esse problemas foram mitigados pela centralização, onde os usuarios envia o trafego para os Provedor de internet, e ele decide a rota, os deixando a merce do provedor de internet, onde o mesmo pode inspecionar seu pacote, manipular ou interceptalo

Diferença do Yggdrasil
O Yggdrasil adota uma abordagem única para roteamento, construindo uma topologia de rede global distribuída. Utiliza uma árvore geradora para sincronização e atribuição de coordenadas aos nós, que trocam filtros de Bloom ( estruturas de dados probabilísticas  utilizadas para testar se um elemento é membro de um conjunto) para compartilhar informações sobre vizinhos alcançáveis. 
Isso permite que os nós intermediários atualizem suas tabelas de roteamento para encaminhar pacotes de forma eficiente. 
Os nós também podem usar o roteamento da árvore geradora para encontrar caminhos mais curtos, recorrendo ao espaço de chaves se necessário. 
Assinaturas criptográficas garantem a segurança das mensagens do protocolo contra adulteração ou falsificação.

Beneficios
Integração de Redes Diversas: Facilidade em conectar redes estáticas ou confiáveis com redes dinâmicas ou não estáticas, sem inundar a rede com grandes quantidades de informações de estado.
Escalabilidade Eficiente: Graças ao uso de conhecimento de roteamento esparso e tráfego de protocolo reduzido, o Yggdrasil é projetado para escalar eficientemente mesmo em redes muito grandes.
Configuração Dinâmica de Caminhos: A rede pode estabelecer e desfazer caminhos rapidamente sem reiniciar todo o processo de roteamento, o que ajuda a lidar eficientemente com eventos como a mobilidade dos nós sem perda significativa de pacotes.

Comparações
YggDrasil 	NÃO deve ser comparado a outros projetos que visam criar sobreposições anonimas como Tor e Lokinet, YggDrasil não tenta e não fornece uma sobreposição de anonimato por design, e sim por conveniencia.

YggDrasil tambem não deve ser comparado com projetos de VPN, pois embora o YGGDrasil possa ser usado para uma especie de "VPN" peer to peer com as devidas configurações, esse não é o objetivo principal do mesmo

YggDrasil tambem não tem a capacidade de fornecer acesso a internet pública ou a outras redes, mas pode ser alcançado com proxies e outras soluções.

