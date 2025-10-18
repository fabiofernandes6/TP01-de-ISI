# Trabalho Prático I - Integração de Sistemas de Informação

## Autor
- **Nome:** Fábio Alexandre Gomes Fernandes
- **Número de Aluno:** 22996

---

## Descrição dos Ficheiros e Pastas

- **`/doc/`**: Contém o relatório final do projeto (`12345_doc.pdf`).
- **`/dataint/`**: Contém os ficheiros do Pentaho Data Integration.
  - `job_principal.kjb`: O Job principal que orquestra todo o processo de ETL.
  - `streaming_netflix.ktr`: A transformação que executa a extração, limpeza, enriquecimento e carregamento dos dados.
- **`/data/input/`**: Contém os datasets de origem utilizados pela transformação.
- **`/data/output/`**: Contém exemplos dos ficheiros gerados pela transformação.
- **`README.md`**: Este ficheiro.

---

## Como Executar a Solução

1.  **Ferramentas Necessárias:**
    - Pentaho Data Integration (Spoon) versão 10.2 (ou a versão que usaste).

2.  **Instruções de Execução:**
    - Abrir a ferramenta Pentaho Data Integration (Spoon).
    - Abrir o ficheiro do Job: `dataint/job_principal.kjb`.
    - Clicar no botão "Play" (Executar) para iniciar o Job.
    - O Job irá verificar se os ficheiros de input existem, executar a transformação `streaming_netflix.ktr` e enviar um email de notificação no final.
    - Os ficheiros de saída serão gerados na pasta `data/output/`.

---

## Vídeo de Demonstração

O vídeo com a demonstração do projeto pode ser acedido através do seguinte link:

**[LINK PARA O TEU VÍDEO NO YOUTUBE/DRIVE/ETC.]**