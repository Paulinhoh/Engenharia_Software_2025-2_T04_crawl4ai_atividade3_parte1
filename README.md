# Engenharia_Software_2025-2_crawl4ai_atividade3_parte1

### Evolução de Software e CI/CD

**Disciplina:** Engenharia de Software II – UFS  
**Turma:** 2025/2 – T04  
**Equipe:** Adriel Menezes Santana - 202100022659 <br>
Luan Feitosa Lima Sátiro - 202300061714 <br>
Luan Prata Mendonça - 202000138885 <br>
Paulo Henrique Carvalho de Andrade - 202200060090 <br>
Paulo Henrique dos Santos Reis - 202100115524 <br>
Thiago Mecena Silva - 202100045840 <br>
Victoria Moura Santos - 202000138900 <br>

---


## Objetivo
Esta atividade tem como objetivo analisar a evolução e pipeline de CI/CD do projeto de software open source crawl4ai, identificando qual a ferramenta de CI/CD utilizado (GitHub Actions, Travis, CircleCI, Jenkins) se houver, e mapear o fluxo, os riscos e possíveis gargalos manuais existentes.

---

## 🚀 Execução no Google Colab

No GitHub, clique no botão
“Open in Colab”:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1Kla9YGVVgcKqJpHyUwq2QLgfiyd1DSbk?usp=sharing#scrollTo=UprBSdTyl0KV)

(ou use o link direto abaixo):

```bash
https://colab.research.google.com/drive/1Kla9YGVVgcKqJpHyUwq2QLgfiyd1DSbk?usp=sharing#scrollTo=UprBSdTyl0KV
```

---

## 🛠️ Configuração e Instalação
1. Instalação das Bibliotecas <br>
Certifique-se de que as bibliotecas necessárias estão instaladas. O notebook já inclui a célula para isso: <br>
`!pip install requests GitPython huggingface_hub`
<br><br>

2. Instale Dependências: Execute a célula (1. Instalação das Bibliotecas).
<br><br>

3. Configuração de Tokens de Acesso
Este projeto requer tokens de API para acessar o GitHub e a Hugging Face. Eles devem ser armazenados de forma segura nos Secrets do Colab (clique no ícone de chave 🔑 na barra lateral esquerda).<br>
`HF_TOKEN`: Seu token de acesso da Hugging Face. Necessário para usar os LLMs.<br>
`GITHUB_TOKEN`: Seu token de acesso pessoal do GitHub. Necessário para acessar a API do GitHub e coletar os commits.
<br><br>

---

## 💡 Como Usar
1. Abra o Google Colab (Disponibilizado acima).<br>
2. Instale Dependências: Execute a célula (1. Instalação das Bibliotecas).<br>
3. Configure Tokens e Parâmetros: Preencha os tokens no Colab Secrets e ajuste os parâmetros GITHUB_OWNER, GITHUB_REPO e COMMITS_TO_FETCH na célula (2. Configurações Iniciais).<br>
4. Execute o Notebook: Execute todas as células do notebook sequencialmente.<br>
5. Visualize os Resultados: A última célula (5. Execução Principal e Visualização de Resultados) irá imprimir as análises de cada LLM diretamente no output do notebook.<br>

---

## 🤖 Modelos de Linguagem Utilizados
Os seguintes LLMs são configurados para análise:
* DeepSeek-V3.2-Exp: `DeepSeek-AI/DeepSeek-V3.2-Exp`
