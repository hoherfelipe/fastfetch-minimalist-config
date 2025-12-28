# 🎨 Fastfetch Minimalist Config

Uma configuração minimalista e elegante para o Fastfetch, otimizada para macOS.


## ✨ Características

- 🎯 Design minimalista e limpo
- 📦 Logo compacto da Apple
- 🎨 Cores suaves e organizadas
- 📊 Informações essenciais do sistema
- 🖥️ Seções bem definidas: Hardware, Software, Environment e Time

## 📋 Pré-requisitos

- [Fastfetch](https://github.com/fastfetch-cli/fastfetch) instalado
- macOS (testado no macOS Tahoe 26.2)

## 🚀 Instalação

### Via Homebrew

```bash
# Instalar o Fastfetch
brew install fastfetch

# Criar diretório de configuração
mkdir -p ~/.config/fastfetch

# Baixar a configuração
curl -o ~/.config/fastfetch/config.jsonc https://raw.githubusercontent.com/SEU_USUARIO/fastfetch-config/main/config.jsonc
```

### Instalação Manual

1. Clone este repositório:
```bash
git clone https://github.com/SEU_USUARIO/fastfetch-config.git
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

## ⚙️ Personalização

O arquivo `config.jsonc` está bem comentado e organizado. Você pode personalizar:

- **Logo**: Ajuste `height`, `width` e `padding` na seção `logo`
- **Cores**: Modifique os valores de `keyColor` (green, yellow, blue, magenta)
- **Módulos**: Adicione ou remova seções conforme necessário
- **Ícones**: Personalize os ícones nas chaves de cada módulo

### Exemplo de customização de cores

```json
{
    "type": "cpu",
    "key": "│ ├󰍛",
    "keyColor": "cyan"  // Mude para sua cor preferida
}
```

## 📸 Screenshots

### Hardware Info
Mostra informações do PC, CPU, GPU e memória de forma compacta.

### Software Info
Exibe sistema operacional, kernel, pacotes instalados e shell.

### Environment
Apresenta informações do ambiente desktop (DE, WM, tema e terminal).

### Time
Mostra idade do sistema, uptime e data/hora atual.

## 🎨 Paleta de Cores

As cores utilizadas seguem o esquema:
- **Verde** (`green`): Hardware
- **Amarelo** (`yellow`): Software  
- **Azul** (`blue`): Environment
- **Magenta** (`magenta`): Time


Configuração criada para ter um fetch minimalista e funcional, mostrando apenas as informações essenciais do sistema.

---


