--- c/Users/clrtj/Desktop/Telegram-HTML/the-cube/README.md
+++ c/Users/clrtj/Desktop/Telegram-HTML/the-cube/README.md
@@ -0,0 +1,88 @@
+# Cubo Zero
+
+**Cubo Zero** é um simulador de Cubo Mágico 3D interativo e de alta performance, desenvolvido para rodar diretamente no navegador. O projeto combina renderização gráfica avançada via WebGL com uma interface de usuário (UI) minimalista e responsiva, oferecendo uma experiência completa tanto para *speedcubers* quanto para entusiastas casuais.
+
+## 📋 Visão Geral do Projeto
+
+O objetivo do Cubo Zero é fornecer uma plataforma digital para a prática de resolução de cubos mágicos, com foco na fidelidade visual, personalização estética e rastreamento de estatísticas de desempenho. A aplicação é construída sobre a biblioteca **Three.js**, garantindo fluidez nas animações e física de rotação.
+
+## 🚀 Funcionalidades Técnicas
+
+### Mecânica do Cubo
+*   **Dimensões Variáveis:** Suporte para múltiplas ordens de complexidade, permitindo alternar entre cubos 2x2, 3x3, 4x4 e 5x5.
+*   **Algoritmo de Embaralhamento:** Sistema de *scramble* configurável (20, 25 ou 30 movimentos) para garantir estados iniciais aleatórios e válidos.
+*   **Física de Rotação:** Três modos de animação de giro configuráveis:
+    *   *Swift:* Rápido e linear.
+    *   *Smooth:* Suave com aceleração/desaceleração.
+    *   *Bounce:* Com efeito elástico ao final do movimento.
+
+### Interface e Visualização
+*   **Câmera Dinâmica:** Alternância entre projeção **Ortográfica** (2D/Isométrica) e **Perspectiva** (3D realista) para melhor adaptação visual do usuário.
+*   **Temas e Personalização:**
+    *   5 temas pré-definidos (*Cube, Erno, Dust, Camo, Rain*).
+    *   Editor de cores granular (HSL - Matiz, Saturação, Luminosidade) para ajuste fino dos materiais do cubo.
+*   **Design Responsivo:** Interface adaptada para dispositivos móveis e desktop, com prevenção de *tap-highlight* e *user-select* para interações de toque otimizadas.
+
+### Sistema de Estatísticas
+O sistema mantém um registro detalhado do desempenho do usuário:
+*   Cronômetro de precisão.
+*   Detecção automática de conclusão ("Solucionado!").
+*   Cálculo de médias móveis (Ao5, Ao12, Ao25).
+*   Registro de melhor e pior tempo.
+
+## 🛠️ Tecnologias Utilizadas
+
+*   **HTML5 Semantic:** Estruturação da aplicação e contêineres de UI.
+*   **CSS3:** Estilização avançada com uso de Flexbox, posicionamento absoluto para *overlays*, transições de opacidade e fontes customizadas (BungeeFont via Base64).
+*   **JavaScript (ES6+):** Lógica de controle de estado e manipulação do DOM.
+*   **Three.js (r95):** Motor gráfico para renderização do ambiente 3D, malhas (meshes), materiais e iluminação.
+
+## 🎨 Aspectos de Design
+
+A interface do usuário (UI) foi projetada para ser não intrusiva. Os menus de configuração (`.ui__prefs`, `.ui__theme`) e estatísticas (`.ui__stats`) operam em camadas sobrepostas ao canvas 3D, utilizando transições suaves para aparecer e desaparecer. A tipografia utiliza a fonte *Bungee*, conferindo um aspecto moderno e geométrico que harmoniza com a natureza cúbica do projeto.
+
+## 🔧 Instalação e Execução
+
+Como se trata de uma aplicação *client-side* estática, não é necessário instalação de dependências de backend.
+
+> **Nota:** Para o carregamento correto de texturas ou fontes locais (se houverem alterações futuras), recomenda-se rodar através de um servidor local (ex: Live Server do VSCode ou Python SimpleHTTPServer) para evitar bloqueios de política CORS.
+
+## 👤 Autor
+
+Desenvolvido por **Cleomar da Silva**.
+&copy; 2025 **NexusCleo**.
+```
