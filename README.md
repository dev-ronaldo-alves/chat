# Chat Seguro P2P · E2EE + ID Duplo 🛡️

Um aplicativo de chat descentralizado, focado em privacidade e segurança, que utiliza a tecnologia **Peer-to-Peer (P2P)** para conexões diretas entre usuários, sem a necessidade de um servidor central para armazenar mensagens.

![Versão](https://img.shields.io/badge/Vers%C3%A3o-2026.1-blueviolet?style=for-the-badge)
![Segurança](https://img.shields.io/badge/Seguran%C3%A7a-E2EE%20Ativo-success?style=for-the-badge)
![Tecnologia](https://img.shields.io/badge/Tecnologia-WebRTC%20%2F%20PeerJS-orange?style=for-the-badge)

## ✨ Funcionalidades Principais

*   **🔒 Criptografia de Ponta a Ponta (E2EE):** Implementação robusta utilizando a Web Crypto API (AES-GCM 256 bits) com derivação de chave via PBKDF2.
*   **🤝 Conexão P2P Direta:** Utiliza WebRTC (via PeerJS) para estabelecer túneis de dados seguros diretamente entre os navegadores.
*   **🆔 Sistema de ID Duplo:**
    *   **ID Fixo:** Um identificador permanente salvo localmente para contatos frequentes.
    *   **ID Descartável:** Um identificador temporário para sessões rápidas e anônimas.
*   **📱 Design Moderno 2026:** Interface intuitiva, dinâmica e otimizada para uso com uma mão (Thumb-friendly), com paleta de cores harmônica e vibrante.
*   **📇 Gestão de Contatos:** Salve IDs de amigos localmente para conexões rápidas.
*   **😊 Emoji Picker Integrado:** Interface dedicada para escolha de emojis sem depender do teclado do sistema.
*   **🧹 Privacidade Total:** Sem banco de dados centralizado. As mensagens existem apenas na memória dos dispositivos conectados e o histórico pode ser limpo instantaneamente.

## 🎨 Design & UI/UX

O projeto segue as melhores práticas de desenvolvimento front-end de 2026:
- **Paleta de Cores:** Combinação de Indigo, Violeta e Coral para uma experiência vibrante.
- **Elevated Neutrals:** Uso de tons neutros sofisticados para reduzir a fadiga visual.
- **Glassmorphism:** Elementos com efeitos de transparência e desfoque de fundo.
- **Micro-interações:** Animações fluidas e feedback visual para cada ação do usuário.

## 🚀 Como Usar

1.  **Acesse o Aplicativo:** Abra o arquivo `index.html` em qualquer navegador moderno.
2.  **Seu ID:** No topo da tela, você verá seu ID atual (Fixo ou Descartável). Clique para copiar e envie para seu amigo.
3.  **Conectar:** Insira o ID do seu amigo no campo "ID do amigo" e clique em **Conectar**.
4.  **Segurança (Opcional):** Clique no ícone de chave ou no badge de criptografia para definir uma **frase secreta compartilhada**. Ambos devem usar a mesma frase para que a criptografia E2EE funcione.
5.  **Chat:** Uma vez conectado, as mensagens serão enviadas diretamente para o outro dispositivo.

## 🛠️ Tecnologias Utilizadas

- **HTML5 / CSS3 (Variáveis modernas & Flexbox/Grid)**
- **JavaScript (ES6+)**
- **[PeerJS](https://peerjs.com/):** Abstração de WebRTC para conexões P2P.
- **[FontAwesome](https://fontawesome.com/):** Ícones vetoriais modernos.
- **Web Crypto API:** Criptografia nativa do navegador de alto desempenho.

## 🛡️ Segurança e Privacidade

Este projeto foi construído com a privacidade como prioridade máxima:
- **Zero Servidor:** Nenhuma mensagem passa por nossos servidores. A sinalização inicial é feita via PeerJS, mas o tráfego de dados é direto entre peers.
- **Local Storage:** Contatos e IDs fixos são armazenados exclusivamente no seu navegador (`localStorage`).
- **E2EE:** Mesmo que alguém intercepte o tráfego P2P, as mensagens estarão protegidas por criptografia AES-GCM se uma frase secreta for definida.

## 📄 Licença

Este projeto está sob a licença MIT. Sinta-se à vontade para usar, modificar e distribuir.

---
*Desenvolvido com foco no futuro da comunicação segura.*
