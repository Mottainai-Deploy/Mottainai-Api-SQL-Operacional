# API Operacional no Render

O Blueprint cria uma API web gratuita usando Docker e a porta 10000. Configure as credenciais privadas no painel, usando o mesmo banco e as chaves corretas do ambiente. Não publique credenciais no Git.

As variáveis adicionais `STAFF_DATA_DECRYPTION_KEYS` e `CUSTOMER_DATA_DECRYPTION_KEYS` podem ser necessárias para ler dados de versões anteriores das chaves; configure-as no painel quando existirem.

O servidor SMTP local e a URL local de recuperação de senha não funcionam no Render: configure SMTP acessível externamente e uma URL pública do fluxo de recuperação antes de usar convites ou redefinições por e-mail. Configure `CORS_ALLOWED_ORIGINS` com as origens HTTPS exatas após publicar os frontends.

Confira o plano Free, os custos e os limites no painel. Após o deploy, teste autenticação Firebase, acesso ao banco e rotas do Operacional com contas autorizadas. O deploy não valida os fluxos automaticamente.
