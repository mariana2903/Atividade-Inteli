# Aprendizado Contínuo 

## Introdução
Modelos de Linguagem Grandes (LMs) são conhecidos por codificar vastas quantidades de conhecimento mundial a partir de seus dados de treinamento, o que é útil para tarefas como resposta a perguntas e diálogo aberto.  No entanto, enfrentam o desafio da renovação do seu conhecimento interno sobre o mundo. À medida que o mundo evolui, novas informações surgem e algumas informações antigas tornam-se desatualizadas. Esse fenômeno, onde as propriedades estatísticas da variável alvo mudam ao longo do tempo, é conhecido como "deriva de conceito".

Sem atualizações regulares, os LMs correm o risco de fornecer informações desatualizadas ou incorretas, o que pode ser problemático em aplicações críticas. Além disso, a atualização desses modelos apresenta desafios técnicos, como o risco de esquecimento catastrófico. Dada a crescente demanda da indústria por modelos adaptativos, é imperativo abordar esses desafios e garantir que os LMs possam refletir com precisão o mundo em constante mudança.

## Solução
### Diagrama de Blocos
<img src="https://github.com/mariana2903/Atividade-Inteli/blob/main/Ponderada-sem9-mod7/Driagrama.drawio.png">

### Descrição dos Blocos
**Conjunto de Dados Inicial**: Este bloco representa o conjunto inicial de dados usados para treinar o modelo pela primeira vez. Geralmente, são grandes conjuntos de texto, muitas vezes extraídos de várias fontes, como livros, artigos, sites, entre outros.

**Modelo Base**: Após o treinamento com os Dados Originais, o modelo adquire uma compreensão inicial do conhecimento mundial. Este bloco representa essa primeira versão treinada do modelo.

**Fluxo de Dados Atualizados**: Este bloco representa dados coletados após o treinamento inicial, refletindo novas informações ou mudanças no conhecimento mundial. Pode incluir notícias recentes, pesquisas atualizadas e outras fontes dinâmicas.

**Detector de concept drift:** Este bloco avaliaria se há uma deriva significativa nos novos dados em comparação com os dados originais ou com o conhecimento do modelo atual.

**Repositório de Conhecimento Intermediário:** Um armazenamento centralizado que combina o conhecimento do Modelo Inicialmente Treinado com os Novos Dados Atualizados. Serve como uma ponte entre o modelo original e o processo de aprendizado contínuo.

**Motor de Atualização CKL:** Este é o núcleo do sistema, responsável por integrar novas informações ao modelo sem esquecer o conhecimento anterior. Utiliza técnicas de aprendizado contínuo para atualizar o modelo com base no Repositório de Conhecimento Intermediário.

**Repositório de Conhecimento Atualizado:** Representa o estado final do conhecimento após o processo de aprendizado contínuo. É a versão mais atualizada e abrangente do modelo, refletindo tanto o conhecimento original quanto as atualizações mais recentes.

## Conclusão
Devido os desafios apresentados e pela forma como as informações globais são atualizadas de forma constante, a capacidade de se atualizar e adaptar Modelos de Linguagem Grandes (LMs) torna-se não apenas desejável, mas essencial. A abordagem de Aprendizado Contínuo de Conhecimento (CKL) surge como uma solução promissora para esse desafio, permitindo que os LMs sejam continuamente treinados e atualizados com novas informações sem perder o conhecimento anterior. A relevância e precisão desses modelos em aplicações do mundo real dependem de sua capacidade de evoluir com o tempo e refletir as mudanças contínuas no conhecimento mundial.

O diagrama ilustra visualmente a complexidade e os passos envolvidos no processo de atualização e é importante entender que cada etapa é essencial e importante no processo. A implementação bem-sucedida do CKL pode ser a chave para garantir que os LMs não apenas atendam às demandas atuais, mas também estejam preparados para as necessidades futuras, mantendo-se relevantes e precisos em um mundo em constante evolução.

## Referências Bibliográficas
JANG, Joel et al. Towards Continual Knowledge Learning of Language Models. 2022. Disponível em: https://arxiv.org/abs/2110.03215. Acesso em: 28/09/2023
