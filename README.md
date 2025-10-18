# Projeto de ETL com Dados da Netflix - Trabalho Prático I de ISI

Este repositório contém todo o material desenvolvido para o primeiro trabalho prático da Unidade Curricular de Integração de Sistemas de Informação (ISI).

---

## 1. Autor

- **Nome:** Fábio Alexandre Gomes Fernandes
- **Número de Aluno:** 22996
- **Email:** a22996@alunos.ipca.pt
- **Curso:** Licenciatura em Engenharia de Sistemas Informáticos
- **Unidade Curricular:** Integração de Sistemas de Informação (ISI)

---

## 2. Descrição dos Ficheiros e Pastas

A estrutura do projeto está organizada da seguinte forma:

- **/dataint/**: Contém os artefactos do Pentaho Data Integration.
  - "project_netflix.kjb": O Job principal que orquestra todo o processo de ETL. É o ficheiro que deve ser executado.
  - "streaming_netflix.ktr": A Transformação que contém toda a lógica de extração, limpeza, validação, correção, enriquecimento e carregamento dos dados.

- **/data/input/**: Contém os ficheiros de dados de origem necessários para a execução do processo.
  - "netflix_activity.csv": Dataset com a atividade de visualização.
  - "netflix_users.csv": Dataset com os dados dos utilizadores, contendo erros para serem limpos e corrigidos pelo processo de ETL.

- **/data/output/**: Contém exemplos dos ficheiros gerados pela execução bem-sucedida do Job.
  - "streaming_users_netflix.csv": O ficheiro principal com os dados de streaming limpos e enriquecidos com os dados dos utilizadores.
  - "relatorio_por_subscricao.csv": O relatório agregado que resume as horas vistas e o número de utilizadores por tipo de subscrição.
  - "relatorio_por_subscricao.json": O mesmo relatório agregado, mas em formato JSON.

- **/doc/**: Contém o relatório final do projeto em formato PDF.
  - "22996_doc.pdf": O documento com toda a teoria, diagramas e conclusões do trabalho.

---

## 3. Como Executar a Solução

Para executar este projeto de ETL, siga os seguintes passos:

1.  **Ferramentas Necessárias:**
    - Pentaho Data Integration (Spoon) - versão 10.2.
    - Acesso a um servidor de email SMTP (configurado no Job para o envio de notificações, por exemplo, Gmail com uma senha de aplicação).

2.  **Preparação:**
    - Garanta que a estrutura de pastas ("dataint", "data/input", etc.) é mantida.
    - Coloque os ficheiros de input ("netflix_activity.csv", "netflix_users.csv") na pasta "/data/input/".

3.  **Execução:**
    - Abra a aplicação Pentaho Data Integration (Spoon).
    - No menu, vá a "File" -> "Open" e selecione o ficheiro do Job: "dataint/project_netflix.kjb".
    - Com o Job aberto, clique no botão "Play" (Executar) na barra de ferramentas principal.

4.  **Resultado Esperado:**
    - O Job irá verificar a existência dos ficheiros de input, executar a transformação, e gerar os ficheiros de output na pasta "/data/output/".
    - No final, será gerado um log da execução e enviado um email de notificação (de sucesso ou de falha) para o endereço configurado.

---

## 4. Vídeo com a Demonstração

O vídeo que demonstra a execução completa do projeto, desde a configuração à visualização dos resultados, pode ser acedido através do seguinte link:

**https://youtu.be/JCH7ZUKThTA**
