---
title: "GEOPROCESSAMENTO"
subtitle: "Desenvolvimento de competências para discussão de processos urbanos por meio de métodos espaciais quantitativos"
author: "Profa. Renata Oliveira"
institute: "Centro Federal de Educação Tecnológica de Minas Gerais"
date: "2020/05/28 (updated: 2020-06-09)"
encoding: "UTF-8"
output:
  xaringan::moon_reader:
    css:  ["mytheme.css", "mytheme-fonts.css"]
    lib_dir: libs
    chakra: libs/remark-latest.min.js
    nature:
      highlightStyle: github
      highlightLines: true
      titleSlideClass: [center, middle, inverse]
      ratio: '16:9'
      slideNumberFormat: |
        <div class="progress-bar-container">
          <div class="progress-bar" style="width: calc(%current% / %total% * 100%);">
          </div>
        </div>`

---

class: center, middle

# SEJAM BEM VINDOS!

---
class: inverse, center, middle

# Retrospecto: 
 - Introdução ao R e ao RStudio
 - Processos Urbanos

---
# Definição
Conjunto de ferramentas usadas para  coleta e tratamento de informações espaciais, geração de saídas na forma de mapas, relatórios, arquivos digitais, etc;
 Deve prover recursos para sua armazenagem, gerenciamento, manipulação e análise. 
Geoprocessamento representa qualquer tipo de processamento de dados georeferenciados (conceito muito mais abrangente).
Um SIG é capaz de processar dados gráficos e não gráficos (alfanuméricos), com ferramentas de análises espaciais e modelagens de superfícies.

Burrough 
“Conjunto poderoso de ferramentas para coletar, armazenar, recuperar, transformar e visualizar dados sobre o mundo real”
Cowen
“Um sistema de suporte à decisão que integra dados referenciados espacialmente num ambiente de respostas a problemas”
Smith
“Um banco de dados indexados espacialmente, sobre o qual opera um conjunto de procedimentos para responder a consultas sobre entidades espaciais”


---
# Cartografia x geoprocessamento
Um programa de SIG é um programa de computador projetado para fazer o computador pensar que é um mapa.

A diferença entre um mapa e um programa SIG é que o segundo é mais inteligente. Você pode perguntar e ele responde.

adaptado de Kennedy, M. 2006 Introducing Geographic Information Systems with ArcGIS

A geocodificação é o que permite transformar dados de localização como coordenadas, endereços e nomes de estabelecimentos em uma geolocalização com latitude e longitude


---
# Por que fazer cartografia digital?
Fazer mapas mais rapidamente.
Fazer mapas mais baratos.
Fazer mapas para usos específicos.
Fazer mapas em situações em que não há disponibilidade de pessoal especializado
Permitir experimentos com representações espaciais diversas dos mesmos dados.
Facilitar atualização de mapas.
Facilitar análises de dados que exigem interação entre estatística e mapas.
Minimizar a necessidade de mapas em papel.
Fazer mapas que não podem ser representados em papel, como em 3D, por exemplo.


---
# Estrutura do shapefile
.dbf – Banco de dados – Informações dos atributos das feições
.prj – Sistemas de coordenadas geográficas
.snb e .sbx – Armazenam os índices espaciais das feições
.shp – Armazenam a geometria das feições
.shx – Armazena o índice da geometria das feições – busca rápida
xml: metadadoem formato XML


