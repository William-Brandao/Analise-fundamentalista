# Projeto de Análise Quantitativa Fundamentalista para Ações da B3

Este projeto implementa um pipeline completo e automatizado para análise quantitativa fundamentalista de ações listadas na B3 (Bolsa de Valores do Brasil). O objetivo é avaliar, ranquear e simular carteiras de investimento com base em indicadores contábeis clássicos, utilizando dados financeiros trimestrais e preços históricos de fechamento.

## Principais Etapas do Pipeline

- **Coleta Automatizada de Dados:**  
    Extração de dezenas de variáveis financeiras trimestrais via API e leitura de preços históricos de ações.

- **Engenharia de Features:**  
    Cálculo de indicadores fundamentais (ROE, ROA, Margem EBITDA, Liquidez, etc.) para padronização e robustez analítica.

- **Ranking Quantitativo:**  
    Sistema de ranqueamento dinâmico com janela móvel (3 anos para avaliação, 1 ano para teste), normalização dos indicadores e cálculo de notas compostas.

- **Simulação de Carteiras:**  
    Comparação entre uma carteira quantitativa (alocação baseada em fundamentos) e uma carteira igualitária (pesos iguais), com reinvestimento dos retornos ao longo dos anos.

- **Visualização e Relatórios:**  
    Geração de gráficos interativos (Plotly, Matplotlib) e relatório técnico em PDF, documentando metodologia, resultados e discussão executiva.

## Tecnologias Utilizadas

- **Python** (Pandas, Numpy, Scikit-learn, Matplotlib, Seaborn, Plotly)
- **APIs Financeiras** para coleta de dados fundamentalistas
- **FPDF** para geração de relatórios em PDF
- **Jupyter Notebook** para organização, documentação e reprodutibilidade

## Destaques e Boas Práticas

- **Pipeline modular e automatizado**, fácil de adaptar para outros ativos ou mercados.
- **Tratamento de dados faltantes** e uso seguro de credenciais via variáveis de ambiente.
- **Reprodutibilidade total**: todos os passos documentados e parametrizáveis.
- **Comparação quantitativa vs igualitária**: simulação multi-anos com reinvestimento.
- **Relatório técnico profissional** pronto para entrega executiva.

## Como Executar

1. Configure o arquivo `.env` com sua chave de API.
2. Garanta que os arquivos de cotações estejam no caminho especificado.
3. Execute o notebook sequencialmente para coletar, processar, simular e gerar os outputs.
4. O relatório final será salvo como PDF no diretório do projeto.

## Observações

- O projeto pode ser expandido para incluir variáveis macroeconômicas, setoriais e de sentimento de mercado.
- Recomenda-se revisar o tratamento de dados faltantes e parametrizar caminhos para maior portabilidade.
- O pipeline é adequado para uso profissional, pesquisa acadêmica ou como base para aplicações reais em gestão de portfólio.

---

**Autor:** William Brandão  
**Contato:** [LinkedIn](www.linkedin.com/in/william-brandão-232abb197)
