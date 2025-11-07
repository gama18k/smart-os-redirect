# Smart OS Redirect

[](https://www.google.com/search?q=LICENSE)
[](https://www.google.com/search?q=https://github.com/SEU_USUARIO/smart-os-redirect/graphs/commit-activity)

Um script HTML/JavaScript leve e simples para **redirecionar automaticamente** usuários para URLs específicas com base no seu Sistema Operacional (iOS, Android). Útil para direcionar visitantes de um mesmo link para a loja de aplicativos correta (App Store ou Google Play).

### Como funciona

O script utiliza a propriedade `navigator.userAgent` do navegador para detectar se o usuário está acessando a página a partir de:

1.  **Android:** Redireciona para `LINK_ANDROID`.
2.  **iOS (iPhone/iPad/iPod):** Redireciona para `LINK_IOS`.
3.  **Outros/Fallback (Ex: Desktop):** Redireciona para um URL de fallback, onde o usuário pode escolher manualmente a loja de aplicativos, ou uma página de aviso.

### Configuração

Altere estas variáveis no topo da tag `<script>` para configurar os seus links:

| Variável | Descrição | Exemplo |
| :--- | :--- | :--- |
| `LINK_IOS` | URL de destino para usuários iOS. | `https://apps.apple.com/app/id123456789` |
| `LINK_ANDROID` | URL de destino para usuários Android. | `https://play.google.com/store/apps/details?id=com.myapp` |
| `else` (Fallback) | URL de destino para desktop ou outros. | `https://meuapp.com/pagina-escolha-manual` |
