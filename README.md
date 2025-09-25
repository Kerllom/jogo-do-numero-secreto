![Status ](https://img.shields.io/badge/Status-Em%20desenvolvimento-brightgreen)
# 🎯 Jogo do Número Secreto

Um jogo interativo de adivinhação desenvolvido em JavaScript puro, onde o desafio é descobrir o número secreto entre 1 e 50 com o menor número de tentativas possível.

## ✨ Características

- 🎮 **Interface Intuitiva**: Design limpo e responsivo
- 🗣️ **Feedback por Voz**: Narração em português brasileiro usando ResponsiveVoice
- 🎯 **Sistema de Dicas**: Orientações direcionais para guiar o jogador
- 📊 **Contador de Tentativas**: Acompanhe seu desempenho
- 🔄 **Números Únicos**: Sistema inteligente que evita repetição de números
- ♻️ **Reinício Automático**: Funcionalidade para começar uma nova partida

## 🎲 Como Funciona

1. **Início**: O jogo gera automaticamente um número secreto entre 1 e 50
2. **Tentativa**: Digite seu palpite no campo de entrada
3. **Feedback**: Receba dicas se o número é maior ou menor
4. **Vitória**: Acerte o número e veja quantas tentativas foram necessárias
5. **Reinício**: Clique em "Novo jogo" para uma nova rodada

## 🚀 Funcionalidades Técnicas

### Sistema de Números Únicos
```javascript
// Evita repetição de números até esgotar todas as possibilidades
if (listaDeNumerosSorteados.includes(numeroEscolhido)) {
    return gerarNumeroAleatorio(); // Recursão para novo número
}
```

### Feedback por Voz
```javascript
// Narração automática em português brasileiro
responsiveVoice.speak(texto, 'Brazilian Portuguese Female', {rate:1.2});
```

### Controle de Estado
- **Tentativas**: Contador automático com pluralização inteligente
- **Botões**: Controle de estado (habilitado/desabilitado)
- **Interface**: Atualização dinâmica de conteúdo

## 🛠️ Tecnologias Utilizadas

- **JavaScript ES6+**: Lógica principal e manipulação do DOM
- **HTML5**: Estrutura semântica
- **CSS3**: Estilização e responsividade
- **ResponsiveVoice API**: Síntese de voz

## 📁 Estrutura do Projeto

```
jogo-numero-secreto/
│
├── index.html          # Estrutura HTML
├── style.css           # Estilos e responsividade
├── app.js              # Lógica principal do jogo
└── README.md           # Documentação
```

## 🎯 Principais Funções

| Função | Descrição |
|--------|-----------|
| `gerarNumeroAleatorio()` | Gera números únicos de 1 a 50 |
| `verificarChute()` | Processa tentativas e fornece feedback |
| `exibirTextoNaTela()` | Atualiza interface com voz |
| `reiniciarJogo()` | Reinicia o estado do jogo |

## 🎮 Como Jogar

1. Acesse o jogo no seu navegador
2. Escute a mensagem inicial (ou leia na tela)
3. Digite um número entre 1 e 50
4. Clique em "Chutar"
5. Use as dicas para ajustar sua próxima tentativa
6. Continue até acertar o número secreto!

## 🏆 Desafios e Aprendizados

Este projeto demonstra conceitos importantes:

- **Manipulação do DOM**: Seleção e modificação de elementos
- **Controle de Fluxo**: Condicionais e loops
- **Gerenciamento de Estado**: Variáveis globais e controle de interface
- **Recursão**: Para geração de números únicos
- **APIs Externas**: Integração com ResponsiveVoice
- **UX**: Feedback imediato e acessibilidade

## 🔧 Possíveis Melhorias

- [ ] Níveis de dificuldade (diferentes intervalos)
- [ ] Sistema de pontuação
- [ ] Histórico de partidas
- [ ] Modo multiplayer
- [ ] Personalização de temas
- [ ] Estatísticas detalhadas

## 🤝 Contribuições

Contribuições são bem-vindas! Sinta-se à vontade para:

1. Fazer fork do projeto
2. Criar uma branch para sua feature (`git checkout -b feature/nova-feature`)
3. Fazer commit das mudanças (`git commit -m 'Adiciona nova feature'`)
4. Push para a branch (`git push origin feature/nova-feature`)
5. Abrir um Pull Request

## 📄 Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

---

⭐ **Gostou do projeto?** Deixe uma estrela no repositório!

🐛 **Encontrou um bug?** Abra uma [issue](../../issues) para reportar.

💡 **Tem uma ideia?** Compartilhe nas [discussions](../../discussions)!
