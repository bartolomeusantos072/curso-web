# curso-web
Parece que você está enfrentando um problema com a política de execução do PowerShell. Isso acontece quando a execução de scripts está desabilitada por padrão no seu sistema. Vamos resolver isso juntos!
npm : O arquivo C:\Program Files\nodejs\npm.ps1 não pode ser carregado porque a execução de scripts foi desabilitada neste sistema. Para obter mais informações, consulte about_Execution_Policies em https://go.microsoft.com/fwlink/?LinkID=135170. No linha:1 caractere:1 + npm init -y + ~~~ + CategoryInfo : ErrodeSegurança: (:) [], PSSecurityException + FullyQualifiedErrorId : UnauthorizedAccess

Siga estes passos para habilitar a execução de scripts no PowerShell:

1. **Abra o PowerShell como Administrador**:
   - Clique no menu "Iniciar", digite "PowerShell", clique com o botão direito do mouse e selecione "Executar como Administrador".

2. **Altere a política de execução**:
   - No PowerShell, digite o seguinte comando e pressione "Enter":
     ```powershell
     Set-ExecutionPolicy Unrestricted
     ```
   - Ele perguntará se você tem certeza; digite "S" para confirmar.

Isso deve permitir que você execute scripts no PowerShell. Se precisar retornar à configuração padrão posteriormente, você pode usar o comando:
```powershell
Set-ExecutionPolicy Restricted
```

Espero que isso ajude! Se tiver mais alguma dúvida, estou aqui para ajudar.

