# FloodIQ 🌊

### **Transformando a gestão hidrológica do Brasil com IA, ciência e colaboração aberta.**

![Logo do projeto](images/logo_colorida.png)

---

## 📖 O que é o FloodIQ?

O **FloodIQ** é uma iniciativa open-source focada em democratizar o acesso a dados hidrológicos de alta qualidade no Brasil. Nosso objetivo é criar uma base de dados robusta e padronizada, conectando a complexa hidrologia brasileira a iniciativas globais como o **FloodHub da Google**. **Utilizamos IA** para processar e correlacionar dados, melhorar a previsão de inundações e engajar comunidades e desenvolvedores na criação de soluções escaláveis.

---

### 🌀 Como o FloodIQ funciona: 

O FloodIQ é projetado para **preencher lacunas no monitoramento hidrológico brasileiro**, aumentando a granularidade das bacias hidrográficas e conectando esses dados ao FloodHub da Google. Nosso foco é fortalecer a base de dados que será integrada ao projeto Caravan Project que já faz a conexão com o FloodHub para alertas de inundalão. Aqui está um fluxo resumido do funcionamento do projeto:

![Fluxo do projeto](images/fluxo.png)

### Por que aumentar a granularidade?

A granularidade é essencial para garantir previsões mais precisas e inclusivas. No Brasil, muitas áreas vulneráveis a inundações estão dentro de bacias menores, que os sistemas globais, como o FloodHub, não conseguem mapear adequadamente. Ao aumentar de **1.344 para 4.319 bacias (aumento de 221%)**, o FloodIQ:

1. Amplia a cobertura de alertas: Incluindo bacias menores e sub-bacias negligenciadas.
2. Melhora a precisão: Reduzindo áreas "invisíveis" no sistema global.
3. Protege mais pessoas: Cobertura detalhada significa impacto direto na prevenção de desastres para milhões de brasileiros.

---

## 📂 Estrutura do Repositório

### Diretórios principais:
- `data/`:  
  Diretório principal contendo bases de dados e scripts relacionados ao projeto.  

  - `examples/`: Scripts para carregar e utilizar a base de dados das bacias hidrográficas. 
  - `watersheds/`: Base de dados de bacias hidrográficas organizada em três formatos: individual, por cluster e unificada (formatos: `.shp`, `.shx`, `.dbf`, etc.).  
  - `gauging_station/`: Base de dados das estações de medições fluviométricas e pluviométricas (formato: `.gpkg`).  
  - `streamflow_data/`: Base de dados com séries temporais de vazão fluviométrica por estação.  

- `models/`: Implementações dos algoritmos de IA: 1) correlação de bacias e estações de medição com NSGAII e 2) clusterização de bacias com Balenced K-Means;  
- `scripts/`: Ferramentas de processamento para derivação de atributos (códigos do Caravan Project part 1 e 2)
- `API/`: Uso da API para acesso aos dados de vazão
- `automation`: Processos automatizados para adaptação e preparação dos dados para integração no Caravan Project.
- `docs/`: Documentação técnica do projeto. (EM CONSTRUÇÃO)  
- `environments`: Configurações e ambiente dedicado ao processamento do projeto

### Principais arquivos:
- `README.md`: Este arquivo! 🎉  
- `CONTRIBUTING.md`: Diretrizes detalhadas para contribuições.  
- `LICENSE`: Licença de uso do projeto.  

---

## 🚀 Tecnologias Utilizadas

- **Linguagens:** Python, JavaScript.  
- **IA e Machine Learning:** Algoritmo genético NSGAII, algoritmo clusterização Balenced K-Means e modelo de larga escala GPT-4o  
- **Infraestrutura:** Google Earth Engine, serviços em nuvem.  
- **Bases de Dados:** API do HidroWeb e BHB250 (codificação otto nível 6)

---

## 🛠️ Como Contribuir

Adoramos contribuições! Aqui está como você pode ajudar:  

1. **Reportar Problemas:** Abra uma issue para bugs, ideias ou melhorias.  
2. **Submeter Melhorias:** Faça um fork do projeto, crie uma branch para suas alterações e envie um pull request.  
3. **Engajar-se com a Comunidade:** Participe de discussões, eventos ou colabore no mapeamento de subbacias.  
4. **Expandir Dados:** Adicione séries temporais de vazão para melhorar a precisão dos modelos.

---

### 🚩 Etapas para Contribuir:
1. Fork o repositório.  
2. Clone seu fork:
   ```bash
   git clone https://github.com/seuusuario/FloodIQ.git
   cd FloodIQ
3. Instale as dependências: "pip install -r requirements.txt"
4. Faça suas alterações e teste.
5. Envie um pull request descrevendo o que foi feito.

---

### 📧 Contato:

Dúvidas ou sugestões? Entre em contato conosco:

E-mail: projetofloodiq@gmail.com ou wendsoncarlos09@gmail.com

---

### 🧩 Próximos passos:

- Expandir o projeto para outras regiões da América Latina.
- Integração com novos parceiros e instituições científicas.

---

## License

This project uses code from the [Frederik Kratzert's repository](https://github.com/kratzert/Caravan) licensed under the **BSD 3-Clause License**.

This project itself is licensed under the **GNU General Public License v3.0 (GPL-3.0)**.

---

### 🙌 Agradecimentos

Agradecemos ao Global Shapers João Pessoa, Climate Reality Project pelo apoio fundamental na construção do FloodIQ.

**Junte-se a nós e faça parte desta revolução hidrológica!**
