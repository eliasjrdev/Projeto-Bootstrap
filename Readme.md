# Projeto Bootstrap 

Projeto desenvolvido utilizando **Bootstrap 5** com o objetivo de válidar os conhecimentos obtidos no curso de Bootstrap fornecidos pela PD EAD. 

Para esta atividade, decidi desenvolver uma **plataforma fictícia de cursos online de programação**.


## Páginas que compõe o Projeto

### index.html
Página principal da plataforma.

**Função:**
- Apresentar a plataforma
- Listar os cursos disponíveis
- Exibir os planos disponíveis na plataforma
- Permitir o cadastro dos usuários através de um formulário
- Disponibilizar um formulário para contato
- Permitir que o usuário acesse a dashboard de acompanhamento
- Disponibilizar as redes sociais da plataforma no roda-pé da página

### dashboard.html
Página da **Área do Aluno**.

**Função:**
- Exibir métricas do aluno
- Mostrar alertas informativos
- Listar progresso nos cursos

## Classes Bootstrap Utilizadas

**Classes reponsáveis pelo Grid:** 
- `container:` Cria um contêiner centralizado com largura máxima adaptável ao tamanho da tela.

- `container-fluid:` Cria um contêiner que ocupa 100% da largura da viewport.

- `row:` Define uma linha do grid do Bootstrap, responsável por organizar as colunas horizontalmente.

- `col-*: ` Define o tamanho das colunas de acordo com os breakpoints (col-12, col-md-6, col-lg-3, etc.).

- `g-*:`Controla o espaçamento (gap) entre colunas e linhas (g-3, g-4), substituindo margens manuais.


**Classes Flexbox:** 
- `d-flex:` Transforma o elemento em um contêiner flexível.

- `flex-column:` Alinha os elementos filhos em coluna (verticalmente).

- `justify-content-*:` Controla o alinhamento horizontal dos itens no eixo principal (center, between, start, end).

- `align-items-*:` Controla o alinhamento vertical dos itens no eixo cruzado (center, start, end).


**Classe Navbar:**
- `navbar:` Classe base para criação de barras de navegação.

- `navbar-expand-lg:` Define que o menu será expandido a partir do breakpoint lg.

- `navbar-dark:` Ajusta cores e contraste do menu para fundos escuros.

- `fixed-top:` Fixa a navbar no topo da página durante o scroll.


**Componentes:**  
- `card:` Cria blocos de conteúdo estruturados, estruturas de cards de informações já completas.

- `badge:` Cria badges (pequenos rótulos informativos) já prontos na página

- `alert:` Exibe mensagens de aviso, sucesso ou atenção ao usuário.

- `table:` Estiliza tabelas com o padrão visual do Bootstrap.

- `table-responsive:` Permite rolagem horizontal da tabela em telas menores quando o conteúdo ultrapassa o container.

- `form-control:` Estiliza formulários automaticamente. Campos de input, textarea, email e etc..

- `form-select:` Estiliza campos do tipo select.

- `form-check:` Estiliza checkboxes e radios.

- `input-group:` Permite agrupar inputs com ícones ou textos auxiliares.

- `btn:` Perimite usar botões já prontos do Bootstrap.


**Classes utilitárias:**  
- `text-center:` Usada para centralizar textos horizontalmente.

- `fw-bold:` Aplica peso de fonte em negrito.

- `shadow-sm:` Aplica uma leve sombra aos elementos.

- `rounded:` Aplica cantos arredondados.

- `d-none:` Usada para ocultar um elemento da tela.

- `img-fluid:` Torna imagens responsivas, ajustando automaticamente à largura do container.

## Uso de CSS Próprio

Foi necessário utilizar CSS personalizado nos seguintes casos:

- **Menu mobile sem JavaScript:**  
  Implementado com `checkbox + label`, permitindo abrir e fechar o menu apenas com CSS.

- **Modal de sucesso do cadastro:**  
  Controlado por checkbox e CSS, substituindo o uso de JS.

- **Identidade visual:**  
  Em agluns casos precisei fazer ajustes de cores,  efeitos de hover, e etc... 
  Como no caso da tabela da página principal, por exemplo. Onde precisei sobreescrever o css do Bootstrap para adaptar as cores da tabela
  de forma que essas cores pudessem ficar mais destacadas na cor de fundo que usei na página.

## Principais Dificuldades

- Criar interações (menu e modal) sem JavaScript.
   Nesta etapa eu não sabia como fazer isso sem Js então precisei pesquisar no Github dos meus colegas que já haviam feito essa atividade,
   para entender como eles fizeram, e adaptar para o meu projeto. Foi quando descobri a técnica de usar o Checkbox como gatilho.

- Ajustar a tabela da dashboard no mobile. 
  A principio não estava aparecendo a rolagem lateral na tabela, passei um tempo tentando entender o porque disso estar acontecendo,
  Só depois descobri que o problema era uma extensão do chrome que eu uso para simular o mobile, que não ativava a rolagem lateral mas na verdade ela
  já estava funcionando no navegador normalmente.
 

