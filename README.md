# Teste_Scrum
Validation Code

# Password Reset Demo (Email/SMS) — Python + SQLite
Fluxo didático de **recuperação de senha** por **e‑mail ou celular**, com **OTP (6 dígitos)** e **token de redefinição** de **uso único** e **expiração**.  
Sem frameworks web: apenas **biblioteca padrão** do Python e **SQLite**. Ideal para aulas, POCs ou preparação de integrações.

Recursos
- Solicitação de reset por **e‑mail** _ou_ **celular** (normalização de telefone).
- Envio de **OTP** (6 dígitos) e **link** de redefinição (ambos com expiração).
- **Uso único** do token de redefinição.
- **Limitação de tentativas** de OTP.
- **Hashes seguros**:
  - PBKDF2‑HMAC‑SHA256 para senhas e OTPs.
  - SHA‑256 para o identificador do token (não armazenamos token em claro).
- **CLI completa** (`main.py`) para executar o fluxo ponta‑a‑ponta.
- **Modo DEV** imprime OTP/link e mantém uma “Outbox” de e‑mail/SMS para testes.

 Requisitos
- Python 3.9
- Sem dependências externas.



