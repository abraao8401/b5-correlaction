# Análise de Correlação Multimodal: Relação entre Transcrição de Áudio e Conteúdo Visual em Vídeos

## Descrição do Projeto

Este projeto visa desenvolver uma solução para medir a correlação entre o conteúdo falado de um vídeo (extraído da transcrição de áudio) e os elementos visuais apresentados, com o objetivo de avaliar se a narrativa auditiva está alinhada ao contexto visual mostrado. Essa análise é fundamental para aplicações como revisão automatizada de vídeos educativos, detecção de fake news e geração de metadados descritivos.

O sistema desenvolvido será capaz de calcular um índice de correlação multimodal utilizando **embeddings visuais** e **embeddings textuais**, quantificando a similaridade semântica entre o que é falado e o que é mostrado no vídeo.

## Funcionalidades

- **Análise de Vídeos**: Processamento de quadros do vídeo para extração de características visuais.
- **Reconhecimento Automático de Fala (ASR)**: Transcrição automática do áudio para análise textual.
- **Processamento de Linguagem Natural (NLP)**: Extração de informações semânticas do áudio transcrito.
- **Aprendizado Multimodal**: Integração de embeddings textuais e visuais para avaliação de similaridade entre áudio e vídeo.
- **Avaliação de Correlação**: Cálculo de um índice de correlação entre o conteúdo falado e os elementos visuais, com métricas como Similaridade Cosine e Coeficiente de Correlação de Pearson.
- **Relatórios Automatizados**: Geração de relatórios destacando vídeos com alta ou baixa coerência narrativa entre o conteúdo visual e auditivo.

## Resultados Esperados

- Desenvolvimento de um modelo que calcule um **índice de correlação multimodal** com um coeficiente de concordância superior a 0,75 em vídeos altamente coerentes.
- Extração de embeddings textuais e visuais utilizando modelos pré-treinados como **CLIP** e **BERT**.
- Avaliação utilizando métricas como **Similaridade Cosine**, **Coeficiente de Correlação de Pearson**, e métricas de alinhamento entre texto e imagem.
- Relatório detalhado com exemplos práticos, destacando vídeos coerentes e inconsistentes em termos de narrativa visual e auditiva.

## Possíveis Tecnologias Utilizadas

- **Python**: Linguagem principal para desenvolvimento do sistema.
- **OpenCV**: Para análise de vídeos e extração de quadros.
- **SpeechRecognition**: Para transcrição automática de áudio (ASR).
- **Transformers (BERT)**: Para embeddings textuais e análise semântica do áudio.
- **CLIP (Contrastive Language-Image Pre-Training)**: Para extração de embeddings visuais e integração multimodal.
- **Scikit-learn**: Para construção e avaliação de modelos de aprendizado de máquina.
- **Matplotlib / Seaborn**: Para visualização de resultados e geração de gráficos de correlação.
- **Streamlit**: Para construção da interface do usuário (caso aplicável).
  
## Bibliografia

ABDALI, Sara; SHAHAM, Sina; KRISHNAMACHARI, Bhaskar. Multi-modal Misinformation Detection: Approaches, Challenges and Opportunities. Journal, v. 1, n. 1, p. 1-37, jan. 2016. Artigo 1.

Zuhui Wang, Zhaozheng Yin, and Young Anna Argyris. 2021. Detecting Medical Misinformation on Social Media
Using Multimodal Deep Learning. IEEE Journal of Biomedical and Health Informatics 25, 6 (2021), 2193–2203.
https://doi.org/10.1109/JBHI.2020.3037027
