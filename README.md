***

***RECOMENDAÇÃO PARA COLABORADORES***

***Utilize o seguinte padrão de commit:***

`:emoji: <tipo>(escopo): <descrição>`

***Veja mais detalhes da formatação em: [Commit Patterns](https://dev.to/renatoadorno/padroes-de-commits-commit-patterns-41co)***

***Adicionem os trabalhos utilizados na pasta Bibliografia e a referência ao final do Readme.***

***

# Análise de Correlação Multimodal: Relação entre Transcrição de Áudio e Conteúdo Visual em Vídeos

## Descrição do Projeto

Este projeto visa desenvolver uma solução para medir a correlação entre o conteúdo falado de um vídeo (extraído da transcrição de áudio) e os elementos visuais apresentados, com o objetivo de avaliar se a narrativa auditiva está alinhada ao contexto visual mostrado. Essa análise é fundamental para aplicações como revisão automatizada de vídeos educativos, detecção de fake news e geração de metadados descritivos.

O sistema desenvolvido será capaz de calcular um índice de correlação multimodal utilizando **embeddings visuais** e **embeddings textuais**, quantificando a similaridade semântica entre o que é falado e o que é mostrado no vídeo.

[Diagrama C4](C4-diagrama.png)

## Funcionalidades

- **Análise de Vídeos**: Processamento de quadros do vídeo para extração de características visuais.
- **Reconhecimento Automático de Fala (ASR)**: Transcrição automática do áudio para análise textual.
- **Aprendizado Multimodal**: Integração de embeddings textuais e visuais para avaliação de similaridade entre áudio e vídeo.
- **Avaliação de Correlação**: Cálculo de um índice de correlação entre o conteúdo falado e os elementos visuais, com métricas como Similaridade Cosine e Coeficiente de Correlação de Pearson.
- **Relatórios Automatizados**: Geração de relatórios destacando vídeos com alta ou baixa coerência narrativa entre o conteúdo visual e auditivo.
  
## Fluxo de Dados

- Entrada → O usuário fornece um vídeo.
- Manipulação → O vídeo é processado para extração de frames e transcrição.
- Embeddings → CLIP gera embeddings visuais e textuais
- Similaridade → Calculada entre embeddings textuais e visuais.
- Classificação → O vídeo é classificado como coerente ou inconsistente.
- Saída → Um relatório final é gerado.
- 
## Resultados Esperados

- Desenvolvimento de um modelo que calcule um **índice de correlação multimodal** com um coeficiente de concordância superior a 0,75 em vídeos altamente coerentes.
- Extração de embeddings textuais e visuais utilizando modelos pré-treinados como **CLIP**.
- Avaliação utilizando métricas como **Similaridade Cosine**, **Coeficiente de Correlação de Pearson**, e métricas de alinhamento entre texto e imagem.
- Relatório detalhado com exemplos práticos, destacando vídeos coerentes e inconsistentes em termos de narrativa visual e auditiva.

## Possíveis Tecnologias Utilizadas

- **Jupyter Notebook**: Ambiente para execução do projeto e interface com usuário
- **Python**: Linguagem principal para desenvolvimento do sistema.
- **FFmpeg**: Para manipulação de vídeo (conversão de formato e extração de áudio)
- **OpenCV**: Para análise de vídeos e extração de quadros.
- **Whisper**: Para transcrição automática de áudio (ASR).
- **CLIP (Contrastive Language-Image Pre-Training)**: Para extração de embeddings visuais, textuais e integração multimodal.
- **Scikit-learn**: Para construção e avaliação de modelos de aprendizado de máquina.
- **Matplotlib / Seaborn**: Para visualização de resultados e geração de gráficos de correlação.
- **Streamlit**: Para construção da interface do usuário (caso aplicável).
  
## Bibliografia

ABDALI, Sara; SHAHAM, Sina; KRISHNAMACHARI, Bhaskar. Multi-modal Misinformation Detection: Approaches, Challenges and Opportunities. Journal, v. 1, n. 1, p. 1-37, jan. 2016. Artigo 1.

Zuhui Wang, Zhaozheng Yin, and Young Anna Argyris. 2021. Detecting Medical Misinformation on Social Media
Using Multimodal Deep Learning. IEEE Journal of Biomedical and Health Informatics 25, 6 (2021), 2193–2203.
https://doi.org/10.1109/JBHI.2020.3037027
