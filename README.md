# 📚 AudioBook - Dom Casmurro

> Um projeto educacional de audiobook interativo baseado na obra clássica "Dom Casmurro" de Machado de Assis, desenvolvido com tecnologias web fundamentais.

## 📋 Descrição do Projeto

Este projeto implementa um tocador de audiobook com interface moderna e responsiva, permitindo a reprodução de múltiplos capítulos de "Dom Casmurro". É um ótimo exemplo prático de como integrar HTML, CSS e JavaScript para criar aplicações web funcionais e atraentes.

**Características principais:**
- ▶️ Controle de reprodução (Play/Pause)
- ⏭️ Navegação entre capítulos (Anterior/Próximo)
- 🎵 10 capítulos disponíveis em formato MP3
- 📱 Interface responsiva
- 🎨 Design moderno com gradiente visual
- ⌛ Progresso automático entre capítulos

---

## 🛠️ Tecnologias Utilizadas

| Tecnologia | Versão | Propósito | Documentação |
|-----------|--------|----------|--------------|
| **HTML5** | Latest | Estrutura semântica do projeto | [MDN - HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML) |
| **CSS3** | Latest | Estilização e layout responsivo | [MDN - CSS](https://developer.mozilla.org/pt-BR/docs/Web/CSS) |
| **JavaScript (ES6+)** | Latest | Lógica interativa e manipulação do DOM | [MDN - JavaScript](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript) |
| **Web Audio API** | Latest | Reprodução e controle de áudio | [MDN - Web Audio API](https://developer.mozilla.org/en-US/docs/Web/API/Web_Audio_API) |
| **HTML5 Audio Element** | Latest | Tag nativa para áudio | [MDN - Audio Element](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/audio) |

---

## 📦 Pré-requisitos

Para executar este projeto em sua máquina, você precisará de:

### Requisitos Mínimos

- **Navegador web moderno** (Chrome, Firefox, Safari, Edge - versão atualizada)
- **Sistema Operacional**: Windows, macOS ou Linux
- **Espaço em disco**: ~50 MB (incluindo os arquivos de áudio)

### Softwares Recomendados (Opcional - Apenas para desenvolvimento)

- **Editor de Código**: [Visual Studio Code](https://code.visualstudio.com/) ou similar
- **Git**: Para controle de versão (opcional)
- **Servidor Local**: [Python](https://www.python.org/) ou [Node.js - http-server](https://www.npmjs.com/package/http-server) (para evitar problemas de CORS)

### Compatibilidade de Navegadores

| Navegador | Versão Mínima | Status |
|-----------|--------------|--------|
| Chrome | 60+ | ✅ Suportado |
| Firefox | 55+ | ✅ Suportado |
| Safari | 12+ | ✅ Suportado |
| Edge | 79+ | ✅ Suportado |
| Internet Explorer | 11 | ❌ Não suportado |

---

## 🚀 Como Executar

### Opção 1: Execução Direta (Recomendado para Testes)

1. **Clone ou baixe o repositório**
   ```bash
   git clone https://github.com/seu-usuario/audiobook-dom-casmurro.git
   cd audiobook-dom-casmurro
   ```

2. **Abra o arquivo HTML**
   - Clique duplo em `index.html` no explorador de arquivos, OU
   - Arraste `index.html` para o seu navegador

### Opção 2: Servidor Local com Python (Recomendado para Produção)

**Python 3.x:**
```bash
python -m http.server 8000
```

**Python 2.x:**
```bash
python -m SimpleHTTPServer 8000
```

Acesse: `http://localhost:8000`

### Opção 3: Servidor Local com Node.js

1. **Instale o http-server globalmente:**
   ```bash
   npm install -g http-server
   ```

2. **Execute o servidor:**
   ```bash
   http-server
   ```

3. **Acesse:**
   ```
   http://localhost:8080
   ```

---

## 📁 Estrutura do Projeto

```
AudioBook - Dom Casmurro/
│
├── index.html              # Arquivo principal (HTML semântico)
├── style.css              # Estilos CSS (Responsivo)
├── script.js              # Lógica JavaScript (Controle de reprodução)
├── README.md              # Documentação do projeto
│
├── audios/                # Pasta com capítulos em áudio
│   ├── 1.mp3
│   ├── 2.mp3
│   ├── 3.mp3
│   ├── 4.mp3
│   ├── 5.mp3
│   ├── 6.mp3
│   ├── 7.mp3
│   ├── 8.mp3
│   ├── 9.mp3
│   └── 10.mp3
│
└── imagens/               # Pasta com assets visuais
    └── dom-casmurro.jpeg  # Capa do livro
```

---

## 🎮 Guia de Uso

### Controles Disponíveis

| Controle | Ação |
|----------|------|
| **▶️ Play/Pause** | Reproduz ou pausa o capítulo atual |
| **⏮️ Anterior** | Volta para o capítulo anterior (ou vai para o último se estiver no primeiro) |
| **⏭️ Próximo** | Avança para o próximo capítulo (ou vai para o primeiro se estiver no último) |

### Comportamento Automático

- ✅ Ao terminar um capítulo, o próximo é reproduzido automaticamente
- ✅ O estado (play/pause) é indicado visualmente pelos ícones
- ✅ A interface exibe o número do capítulo e o nome do autor

---

## 💻 Detalhes Técnicos

### Funcionalidades JavaScript Implementadas

**Gerenciamento de Estado:**
- Rastreamento do capítulo atual
- Status de reprodução (tocando/pausado)

**Event Listeners:**
- Clique nos botões de controle
- Finalização automática de áudio (`ended`)

**Manipulação do DOM:**
- Atualização dinâmica do número do capítulo
- Alternância de classes CSS para indicadores visuais

**Estrutura de Dados:**
```javascript
quantidadeCapitulos = 10  // Total de capítulos disponíveis
capitulo = 1              // Capítulo atualmente carregado
taTocando = false         // Status da reprodução
```

---

## 📚 Documentação de Referência

Abaixo estão os principais recursos utilizados no projeto:

### Frontend
- [**MDN Web Docs - HTML**](https://developer.mozilla.org/pt-BR/docs/Web/HTML) - Referência completa de HTML
- [**MDN Web Docs - CSS**](https://developer.mozilla.org/pt-BR/docs/Web/CSS) - Referência completa de CSS
- [**MDN Web Docs - JavaScript**](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript) - Referência completa de JavaScript
- [**HTML5 Audio Element**](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/audio) - Documentação da tag `<audio>`
- [**DOM Events**](https://developer.mozilla.org/pt-BR/docs/Web/Events) - Guia de eventos do DOM

### Ferramentas Recomendadas
- [**Visual Studio Code**](https://code.visualstudio.com/) - Editor de código
- [**Git Documentation**](https://git-scm.com/doc) - Controle de versão
- [**Can I Use**](https://caniuse.com/) - Compatibilidade de navegadores

---

## 🎓 Propósito Educacional

Este projeto foi desenvolvido como exercício de aprendizado em desenvolvimento web, cobrindo:

✅ Estruturação semântica com HTML5  
✅ Estilização responsiva com CSS3  
✅ Interatividade com JavaScript puro (sem frameworks)  
✅ Integração de elementos visuais (SVG, imagens)  
✅ Event handling e gerenciamento de estado  
✅ Integração de mídia (áudio HTML5)  

---

## 👨‍💻 Autor

**Gabriel** - Desenvolvedor

---

## 📝 Licença

Este projeto é fornecido para fins educacionais. A obra "Dom Casmurro" é do domínio público.

---

## 🤝 Contribuições

Sugestões e melhorias são bem-vindas! Sinta-se à vontade para abrir uma issue ou enviar um pull request.

---

## 📞 Suporte

Caso encontre algum problema:

1. Verifique se seu navegador é compatível (veja seção acima)
2. Certifique-se de que os arquivos de áudio estão na pasta `audios/`
3. Tente executar em um servidor local (Python ou Node.js)
4. Limpe o cache do navegador (Ctrl+Shift+Delete)
5. Consulte o console do navegador (F12) para mensagens de erro

---

**Última atualização:** Janeiro de 2026
