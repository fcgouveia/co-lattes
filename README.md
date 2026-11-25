# Venn de códigos ID Lattes ou Co-Lattes

Aplicação web interativa para identificar, comparar e visualizar relações entre conjuntos de pesquisadores a partir de seus códigos de identificação na Plataforma Lattes (CNPq).

A ferramenta permite inserir ou importar listas de códigos ID Lattes, comparar de dois a cinco conjuntos simultaneamente e visualizar suas interseções por meio de diagramas de Venn. Também possibilita explorar os resultados, copiar códigos e exportar os dados para utilização em outras ferramentas de análise.

## Funcionalidades

- **Comparação de conjuntos:** permite trabalhar com 2, 3, 4 ou 5 conjuntos simultaneamente.
- **Identificação de interseções:** identifica códigos ID Lattes compartilhados entre diferentes conjuntos.
- **Diagrama de Venn:** apresenta visualmente as relações de interseção e exclusividade entre os conjuntos.
- **Importação de dados:** permite importar arquivos nos formatos CSV, TXT, JSON, XLSX, XLS, HTML e TSV.
- **Entrada manual:** possibilita colar listas de códigos ou textos que contenham identificadores Lattes.
- **Integração com a busca do CNPq:** gera links para consultas na Busca de Currículos Lattes a partir dos termos informados.
- **Exploração dos resultados:** permite selecionar regiões do diagrama ou linhas da tabela para consultar os códigos correspondentes.
- **Cópia de resultados:** permite copiar os códigos de uma região selecionada.
- **Exportação CSV:** permite copiar uma tabela com os códigos e sua distribuição entre os conjuntos.
- **Exportação SVG:** permite copiar o diagrama de Venn em formato vetorial.
- **Interface adaptável:** possui suporte a temas claro e escuro, além de adaptação a diferentes tamanhos de tela.

## Como utilizar

### 1. Acessar a aplicação

Abra o arquivo HTML em um navegador atualizado. Não é necessária instalação de servidor ou ambiente de desenvolvimento.

### 2. Definir os conjuntos

Selecione a quantidade de conjuntos que deseja comparar: 2, 3, 4 ou 5.

### 3. Identificar os conjuntos

Para cada conjunto:

1. Informe um nome de identificação.
2. Digite um termo de busca.
3. Informe o parâmetro de busca utilizado pelo CNPq (por padrão, `ASSUNTO`).
4. Utilize o botão **Abrir busca no CNPq** para acessar a consulta correspondente.

### 4. Inserir os códigos ID Lattes

Os códigos podem ser inseridos de duas maneiras:

- Colando diretamente os códigos ou textos que os contenham na área de texto de cada conjunto.
- Importando arquivos nos formatos disponibilizados pela aplicação.

O sistema identifica automaticamente os códigos e elimina duplicações dentro de cada conjunto.

São reconhecidos dois padrões de identificadores:

- Códigos no formato `K0000000A0`.
- Sequências numéricas de 16 dígitos.

### 5. Analisar os resultados

Após inserir os dados, a aplicação gera automaticamente:

- O diagrama de Venn;
- A quantidade de códigos únicos em cada conjunto;
- A quantidade de códigos em cada região de interseção;
- Uma tabela com as combinações identificadas.

Clique nos números do diagrama ou nas linhas da tabela para visualizar os códigos correspondentes.

### 6. Exportar os resultados

A aplicação disponibiliza três opções:

- **Copiar códigos:** copia os códigos da região selecionada.
- **Copiar tabela (CSV):** copia a distribuição dos códigos entre os conjuntos.
- **Copiar SVG:** copia o diagrama de Venn em formato vetorial.

## Tecnologias utilizadas

O projeto foi desenvolvido como uma aplicação web independente, utilizando:

- **HTML5:** estrutura da aplicação.
- **CSS3:** estilos, responsividade e temas visuais.
- **JavaScript:** processamento dos dados, identificação das interseções e geração do diagrama.
- **SVG:** representação gráfica do diagrama de Venn.
- **LZ-String:** compactação de parâmetros utilizados na construção dos links de busca do CNPq.
- **SheetJS (XLSX):** leitura e processamento de arquivos Excel.

As bibliotecas LZ-String e SheetJS são carregadas por meio de CDNs.

## Aplicações potenciais

A ferramenta pode ser utilizada em pesquisas bibliométricas, estudos de prosopografia acadêmica, análises de redes de pesquisadores e investigações sobre a distribuição de competências e temas de pesquisa.

Entre as possibilidades de aplicação estão:

- Comparar pesquisadores associados a diferentes temas de investigação.
- Identificar pesquisadores que atuam simultaneamente em áreas distintas.
- Investigar interfaces entre campos científicos.
- Identificar grupos de pesquisadores compartilhados entre diferentes consultas na Plataforma Lattes.
- Apoiar a construção de conjuntos de pesquisadores para análises posteriores.

## Limitações e observações

- A aplicação trabalha com códigos de identificação ID Lattes, não realizando, por si só, a coleta ou a análise integral dos currículos.
- Os resultados dependem dos códigos fornecidos ou importados pelo usuário.
- A busca de currículos é realizada por meio de links para a plataforma do CNPq; a aplicação não executa coleta automática de dados nessa plataforma.
- O reconhecimento dos identificadores depende dos padrões previstos no código.
- A representação geométrica do diagrama é uma aproximação visual. Regiões que não possam ser representadas adequadamente no desenho continuam disponíveis na tabela de resultados.

## Execução e publicação

Por ser uma aplicação desenvolvida em HTML, CSS e JavaScript, não exige instalação de dependências locais.

Para executar:

1. Baixe ou clone este repositório.
2. Abra o arquivo HTML em um navegador atualizado.
3. Utilize a aplicação diretamente.

Também é possível disponibilizar a ferramenta publicamente por meio do **GitHub Pages**.

## Créditos e desenvolvimento

O código-fonte desta aplicação foi desenvolvido com auxílio de inteligência artificial generativa, utilizando o **Claude Sonnet 5.5**, como ferramenta de apoio à programação e à implementação das funcionalidades.

## Licença

Este projeto é disponibilizado publicamente sob uma licença de uso não comercial (Non-Commercial License).

É permitido utilizar, estudar, modificar e redistribuir o código para fins pessoais, acadêmicos, científicos e educacionais, desde que sejam mantidos os créditos de autoria e os termos desta licença.

O uso comercial, incluindo a comercialização, incorporação em produtos ou serviços comerciais e exploração econômica da aplicação, depende de autorização prévia e expressa do titular dos direitos autorais.

Para solicitar autorização de uso comercial ou obter uma licença comercial, entre em contato com o titular do projeto.

O software é fornecido "no estado em que se encontra" ("as is"), sem garantias de qualquer natureza, expressas ou implícitas, incluindo, mas não se limitando a, garantias de comercialização, adequação a uma finalidade específica e não violação de direitos de terceiros.

Em nenhuma circunstância os autores ou titulares dos direitos autorais serão responsáveis por quaisquer reclamações, danos ou outras responsabilidades, sejam elas decorrentes de contrato, ato ilícito ou qualquer outra forma, relacionadas ao software, ao seu uso ou a outras operações realizadas com o software.
