
# Checklist – Publicação do Holocron TIC no Microsoft Copilot Studio

## Pré-requisitos
- Acesso ao Copilot Studio e permissões para publicar.
- Arquivo `memoria-licitacao-tic.md` validado (versão e seções conferidas).
- Conectores (SharePoint/OneDrive) habilitados, se usar leitura dinâmica da memória.

## Passo a passo
1. **Criar o Copilot**  
   - Acesse https://copilotstudio.microsoft.com → **Criar > Novo Copilot**.  
   - Nome: "Holocron TIC – NUTEC/SJMA
   - Descrição: “Especialista em contratações e licitações de TIC para o NUTEC/SJMA, com escopo fechado conforme memória.”

2. **Configurar Instruções**  
   - Menu **Configurações > Instruções do Copilot**.  
   - Cole o prompt de sistema de "Holocron TIC" (arquivo `prompt-agente-Holocron-TIC.txt`).  
   - No final, inclua o conteúdo atualizado do `memoria-licitacao-tic.md` **OU** configure conector para leitura.

3. **Adicionar a Memória**  
   - Opção A: copiar o conteúdo do arquivo para o final do prompt.  
   - Opção B (recomendada): **Conector SharePoint/OneDrive** apontando para o arquivo, para atualização sem republicação.

4. **Políticas e Escopo Fechado**  
   - Desativar uso de fontes externas.  
   - Desabilitar respostas criativas; manter tom objetivo.  
   - Ativar checagem de conteúdo sensível.

5. **Testes**  
   - Rodar os Q&A canônicos da memória (§7).  
   - Fazer perguntas fora do escopo (deve recusar conforme modelo).  
   - Verificar citações de seções/IDs.

6. **Publicação**  
   - **Publicar** e selecionar canais (Teams/Web/Power Apps).  
   - Definir permissões (grupo de licitações TIC).  
   - Registrar versão publicada (anotar hash/data).

7. **Operação e Evolução**  
   - Manter changelog e controle de versões.  
   - Ao atualizar a memória, repetir testes canônicos.  
   - Registrar gaps em §10 da memória.

## Dicas
- Mantenha IDs estáveis para normas/modelos.  
- Use linguagem simples com o prefixo “Simplificadamente:” quando necessário.  
- Não responda sem ancoragem explícita na memória.
