# 🧠 Análise de Sentimentos com Language Studio - Azure AI

Este repositório documenta a prática realizada com o **Language Studio** da Microsoft Azure, com foco na **Análise de Sentimentos**. A atividade faz parte do laboratório da DIO sobre soluções de IA baseadas em linguagem natural.

## 🎯 Objetivo

Utilizar o **Language Studio** para aplicar análise de sentimentos em textos variados, identificando emoções expressas — como **positivas**, **negativas**, **neutras** ou **mistas** — com base no modelo pré-treinado da Microsoft.

---

## 🛠️ Passos Realizados

1. **Acesso ao Language Studio**
   - Plataforma: [https://language.azure.com/](https://language.azure.com/)
   - Navegação: Menu "Analisar texto" > "Análise de Sentimento"

2. **Entrada de Texto**
   - Textos utilizados como exemplo:
     - _"Estou muito feliz com o atendimento que recebi hoje!"_
     - _"O produto chegou com defeito e ninguém respondeu meus e-mails."_
     - _"Não foi bom, nem ruim. Apenas ok."_

3. **Configurações**
   - Idioma: `Português (pt)`
   - Tipo de entrada: Frase única ou múltiplas frases
   - Modelo: Pré-treinado (padrão da plataforma)

4. **Resultado Obtido**
   - A plataforma retorna um JSON com:
     - **Classificação geral do sentimento**
     - **Pontuação por tipo (positivo, neutro, negativo)**
     - **Análise detalhada por frase**

   #### Exemplo de saída:
   ```json
   {
     "documentSentiment": "positive",
     "confidenceScores": {
       "positive": 0.97,
       "neutral": 0.03,
       "negative": 0.00
     }
   }
