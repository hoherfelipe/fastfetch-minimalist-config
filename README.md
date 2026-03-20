# Fastfetch Minimalist Config

Uma configuração minimalista e elegante para o Fastfetch, otimizada para macOS.

<img width="1151" height="558" alt="image" src="<img width="1206" height="1000" alt="image" src="https://github.com/user-attachments/assets/cf8598dc-31d6-4daa-bdfa-0933f2ec47ca" />
" />



##  Características

- 🎯 Design minimalista e limpo
- 📦 Logo compacto da Apple
- 🎨 Cores suaves e organizadas
- 📊 Informações completas do sistema
- 💾 Monitoramento de disco com uso e porcentagem
- 🔋 Status da bateria com temperatura
- 🖥️ Seções bem definidas: Hardware, Software, Environment e Time
- ⚡ Formatação alinhada e consistente


## 📋 Pré-requisitos

- [Fastfetch](https://github.com/fastfetch-cli/fastfetch) instalado
- macOS (testado no macOS Tahoe 26.2)
- Nerd Font instalada no terminal (recomendado para ícones)

## 🚀 Instalação

### Via Homebrew

```bash
# Instalar o Fastfetch
brew install fastfetch

# Criar diretório de configuração
mkdir -p ~/.config/fastfetch

# Baixar a configuração
curl -o ~/.config/fastfetch/config.jsonc https://raw.githubusercontent.com/hoherfelipe/fastfetch-config/main/config.jsonc
```

### Instalação Manual

1. Clone este repositório:
```bash
git clone https://github.com/hoherfelipe/fastfetch-config.git
cd fastfetch-config
```

2. Copie o arquivo de configuração:
```bash
mkdir -p ~/.config/fastfetch
cp config.jsonc ~/.config/fastfetch/config.jsonc
```

3. Execute o Fastfetch:
```bash
fastfetch
```

##  Ícones Nerd Fonts
Esta configuração utiliza ícones do Nerd Fonts para uma aparência mais elegante. Para visualizar os ícones corretamente:
Instalar Nerd Font
```bash
# Via Homebrew
brew tap homebrew/cask-fonts

# Escolha uma das fontes:
brew install font-hack-nerd-font
# ou
brew install font-jetbrains-mono-nerd-font
# ou
brew install font-fira-code-nerd-font
```

### Configurar no iTerm2

Abra o iTerm2
Vá em Preferences (Cmd + ,)
Profiles → Text
Font → Escolha uma Nerd Font instalada

Buscar mais ícones
Todos os ícones utilizados nesta configuração podem ser encontrados em:
https://www.nerdfonts.com/cheat-sheet
Você pode pesquisar por nome, copiar o ícone e colar diretamente no arquivo config.jsonc.

##  Personalização

O arquivo `config.jsonc` está bem comentado e organizado. Você pode personalizar:

- **Logo**: Ajuste `height`, `width` e `padding` na seção `logo`
```bash
"logo": {
    "type": "builtin",
    "height": 8,      // Altura do logo
    "width": 12,      // Largura do logo
    "padding": {
        "top": 1,     // Espaçamento superior
        "left": 2     // Espaçamento esquerdo
    }
}
```
- **Cores**: Modifique os valores de `keyColor` (green, yellow, blue, magenta)
```bash
{
    "type": "cpu",
    "key": "│ ├󰍛",
    "keyColor": "green"  // Opções: green, yellow, blue, magenta, cyan, red
}
```
- **Separador**: O separador padrão é : (espaço + dois pontos + espaço)
```bash
"display": {
    "separator": " : "  // Customize como preferir
}
```
- **Ícones**: Personalize os ícones nas chaves de cada módulo.

- **Módulo de Disco**: Formato customizado sem flags extras 
```bash
{
    "type": "disk",
    "key": "│ ├",
    "keyColor": "green",
    "format": "{1} / {2} ({3}) - {9}"  // Usado / Total (%) - Sistema
}
```
Placeholders disponíveis:
- {1} = Espaço usado
- {2} = Espaço total
- {3} = Porcentagem
- {9} = Sistema de arquivos (apfs, ext4, etc)


- **Módulo da Bateria**: Com suporte a temperatura
```bash
{
    "type": "battery",
    "key": " Battery",
    "keyColor": "cyan",
    "temp": true  // Mostra temperatura da bateria
}
```
## 

## Seções

### Hardware Info
- Informações sobre o computador:
- PC/Host (modelo do Mac)
- CPU com ícone
- GPU com ícone
- Memória RAM com uso e porcentagem
- Disco com uso, total e porcentagem

### Software Info
- Informações do sistema operacional:
- OS (sistema operacional e versão)
- Kernel (versão do Darwin)
- Packages (pacotes brew e brew-cask)
- Shell (shell utilizado)

### Environment
- Ambiente desktop:
- DE (Desktop Environment)
- Login Manager
- Window Manager
- WM Theme (tema do sistema)
- Terminal (aplicativo de terminal)

### Time
- Informações temporais:
- OS Age (idade da instalação do sistema)
- Uptime (tempo ligado)
- Date (data e hora atual)
## 

##  Paleta de Cores

As cores utilizadas seguem o esquema:
- **Verde** (`green`): Hardware
- **Amarelo** (`yellow`): Software  
- **Azul** (`blue`): Environment
- **Magenta** (`magenta`): Time
## 

### Contribuindo
Contribuições são bem-vindas! Sinta-se à vontade para:

Fazer um fork do projeto
Criar uma branch para sua feature (git checkout -b feature/MinhaFeature)
Commit suas mudanças (git commit -m 'Adiciona MinhaFeature')
Push para a branch (git push origin feature/MinhaFeature)
Abrir um Pull Request

### Inspiração
Configuração criada para ter um fetch minimalista e funcional, mostrando informações essenciais do sistema de forma elegante e organizada.

---


