# Weather App 🌤️

Uma aplicação desktop simples e intuitiva para consultar informações meteorológicas em tempo real de qualquer cidade do mundo.

## 📝 Descrição

Este é um aplicativo de clima desenvolvido em Python usando PyQt5 para a interface gráfica e a API do OpenWeatherMap para obter dados meteorológicos atualizados. A aplicação apresenta uma interface limpa e moderna com emojis representativos para diferentes condições climáticas.

## ✨ Funcionalidades

- 🏙️ **Busca por cidade**: Digite o nome de qualquer cidade do mundo
- 🌡️ **Temperatura atual**: Mostra a temperatura em Celsius
- 🌈 **Emojis visuais**: Representação visual das condições climáticas
- 📄 **Descrição detalhada**: Descrição textual das condições meteorológicas
- ❌ **Tratamento de erros**: Mensagens de erro claras e específicas
- 🎨 **Interface moderna**: Design limpo e responsivo

## 🛠️ Tecnologias Utilizadas

- **Python 3.x**
- **PyQt5** - Interface gráfica
- **Requests** - Requisições HTTP para a API
- **OpenWeatherMap API** - Dados meteorológicos

## 📋 Pré-requisitos

Antes de executar a aplicação, certifique-se de ter:

1. Python 3.6 ou superior instalado
2. Conexão com a internet
3. As dependências necessárias instaladas

## 🚀 Instalação e Execução

### 1. Clone ou baixe o projeto

```bash
git clone https://github.com/FelipeRuizMarcuci/weather-app.git
cd weather-app
```

### 2. Instale as dependências

```bash
pip install PyQt5 requests
```

### 3. Execute a aplicação

```bash
python main.py
```

## 🎯 Como Usar

1. **Abra a aplicação**: Execute o comando `python main.py`
2. **Digite o nome da cidade**: No campo de entrada, digite o nome da cidade desejada
3. **Clique em "Get Weather"**: Pressione o botão para buscar as informações
4. **Visualize os resultados**: A aplicação mostrará:
   - Temperatura atual em Celsius
   - Emoji representativo da condição climática
   - Descrição textual do clima

### Exemplo de uso:

- Digite: "São Paulo"
- Resultado: "25°C ☀️ Clear sky"

## 🌦️ Condições Climáticas Suportadas

A aplicação reconhece e exibe emojis para diferentes condições:

- ⛈️ **Tempestade** (200-299): Trovoadas
- 🌦️ **Garoa** (300-399): Chuva leve
- 🌧️ **Chuva** (500-599): Precipitação
- ❄️ **Neve** (600-699): Neve
- 🌫️ **Neblina** (700-799): Condições atmosféricas
- ☀️ **Sol** (800): Céu limpo
- ☁️ **Nuvens** (801-899): Céu nublado
- ❓ **Desconhecido**: Outras condições

## 🔑 Configuração da API

A aplicação utiliza a API gratuita do OpenWeatherMap. A chave da API já está configurada no código, mas para uso em produção, recomenda-se:

1. Criar uma conta em [OpenWeatherMap](https://openweathermap.org/api)
2. Obter sua própria chave da API
3. Substituir a chave no código na linha 62:
   ```python
   api_key = "sua_chave_aqui"
   ```

## ⚠️ Tratamento de Erros

A aplicação possui tratamento robusto de erros para diferentes situações:

- **400 - Bad Request**: Nome da cidade inválido
- **401 - Unauthorized**: Chave da API inválida
- **403 - Forbidden**: Acesso negado
- **404 - Not Found**: Cidade não encontrada
- **500 - Internal Server Error**: Erro do servidor
- **502 - Bad Gateway**: Resposta inválida do servidor
- **503 - Service Unavailable**: Serviço indisponível
- **504 - Gateway Timeout**: Timeout do servidor
- **Erros de Conexão**: Problemas de conectividade
- **Timeout**: Tempo limite de requisição excedido

## 🎨 Personalização

### Estilos CSS

A aplicação utiliza estilos CSS customizados para:

- Fonte: Calibri para textos gerais
- Fonte de emojis: Segoe UI Emoji
- Tamanhos de fonte responsivos
- Cores e alinhamentos

### Modificações Possíveis

- Alterar cores no stylesheet
- Adicionar novos campos de informação
- Modificar emojis para condições climáticas
- Implementar histórico de pesquisas
- Adicionar previsão estendida

## 📱 Interface

A aplicação possui uma interface simples e intuitiva:

```
┌─────────────────────────────────┐
│        Enter city name:         │
│  ┌─────────────────────────────┐ │
│  │     [Campo de entrada]      │ │
│  └─────────────────────────────┘ │
│  ┌─────────────────────────────┐ │
│  │      [Get Weather]          │ │
│  └─────────────────────────────┘ │
│                                 │
│            25°C                 │
│             ☀️                  │
│         Clear sky               │
└─────────────────────────────────┘
```

## 👨‍💻 Autor

**Felipe Ruiz Marcuci**

- GitHub: [@FelipeRuizMarcuci](https://github.com/FelipeRuizMarcuci)
