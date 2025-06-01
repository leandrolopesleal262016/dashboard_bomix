# Dashboard Bomix - Análise Inteligente de Produção

![Dashboard Bomix](https://img.shields.io/badge/Status-Concluído-brightgreen) ![Versão](https://img.shields.io/badge/Versão-1.0-blue) ![Licença](https://img.shields.io/badge/Licença-MIT-yellow)

## 📊 Visão Geral

O Dashboard Bomix é uma aplicação web completa desenvolvida para análise inteligente de dados de produção. O sistema processa arquivos Excel contendo informações de pedidos e controle de rótulos, apresentando visualizações interativas e métricas essenciais para tomada de decisões.

## ✨ Funcionalidades Principais

### 📈 Visualizações Interativas
- **Gráfico de Status dos Pedidos**: Distribuição visual dos pedidos por status (Liberado, Pendente, Em Atraso)
- **Top 5 Clientes**: Ranking dos principais clientes por volume de pedidos
- **Evolução Mensal**: Análise temporal dos pedidos por mês
- **Status dos Rótulos**: Controle visual do status dos rótulos (No Prazo, Vencido, Próximo do Vencimento)

### 🔍 Sistema de Filtros
- Filtro por Status do pedido
- Filtro por Cliente
- Filtro por Estado
- Aplicação dinâmica com atualização automática das visualizações

### 📊 Métricas em Tempo Real
- Total de Pedidos
- Pedidos Liberados
- Valor Total Processado
- Quantidade de Tipos de Rótulos

### 📋 Tabelas Detalhadas
- **Pedidos Recentes**: Últimos 20 pedidos com informações completas
- **Controle de Rótulos**: Gerenciamento de rótulos com status e validades

## 🚀 Como Usar

### 1. Preparação do Arquivo Excel
Certifique-se de que seu arquivo Excel contenha as seguintes abas:
- **Check PCP**: Dados dos pedidos com colunas como Status, Cliente, Estado, Data Entrega, etc.
- **Relatório de Rótulos (BI)**: Informações sobre rótulos, status e validades

### 2. Carregamento dos Dados
1. Acesse o dashboard através do arquivo `index.html`
2. Clique no botão "📁 Carregar Arquivos" no menu superior
3. Selecione seu arquivo Excel (.xlsx ou .xls)
4. Aguarde o processamento automático dos dados

### 3. Navegação e Análise
- Use os filtros para segmentar os dados conforme necessário
- Analise as métricas nos cards superiores
- Explore os gráficos interativos
- Consulte as tabelas detalhadas para informações específicas

## 🛠️ Tecnologias Utilizadas

- **HTML5**: Estrutura semântica da aplicação
- **CSS3**: Estilização moderna com gradientes e efeitos visuais
- **JavaScript ES6+**: Lógica de processamento e interatividade
- **Chart.js**: Biblioteca para criação de gráficos interativos
- **SheetJS (XLSX)**: Processamento de arquivos Excel
- **Design Responsivo**: Compatível com desktop, tablet e mobile

## 📱 Responsividade

O dashboard é totalmente responsivo e otimizado para:
- **Desktop**: Experiência completa com todas as funcionalidades
- **Tablet**: Layout adaptado para telas médias
- **Mobile**: Interface otimizada para smartphones

## 🎨 Design e UX

### Características Visuais
- **Tema Moderno**: Paleta de cores profissional com azul corporativo (#1e3a5f)
- **Glassmorphism**: Efeitos de vidro e transparência
- **Micro-animações**: Transições suaves e hover effects
- **Cards Interativos**: Elementos que respondem à interação do usuário

### Usabilidade
- Interface intuitiva e fácil navegação
- Carregamento automático do arquivo padrão quando disponível
- Feedback visual durante o processamento
- Mensagens de boas-vindas para novos usuários

## 📊 Estrutura de Dados Esperada

### Aba "Check PCP"
| Campo | Descrição | Tipo |
|-------|-----------|------|
| Status | Status do pedido (LIBERADO, PENDENTE, etc.) | Texto |
| PedidoVenda_ID | Identificador único do pedido | Texto/Número |
| Cliente | Nome do cliente | Texto |
| Estado | Estado de destino | Texto |
| DataEntrega | Data prevista de entrega | Data |
| Quantidade | Quantidade do pedido | Número |
| ValorUnitario | Valor unitário do item | Número |
| Emissao | Data de emissão do pedido | Data |

### Aba "Relatório de Rótulos (BI)"
| Campo | Descrição | Tipo |
|-------|-----------|------|
| ID | Identificador do rótulo | Texto/Número |
| Rotulo | Descrição do rótulo | Texto |
| Status | Status do rótulo | Texto |
| SaldoTotal | Saldo total disponível | Número |
| QtdPedido | Quantidade pedida | Número |
| DataValidade | Data de validade | Data |

## 🔧 Instalação e Configuração

### Requisitos
- Navegador web moderno (Chrome, Firefox, Safari, Edge)
- Arquivo Excel com estrutura compatível

### Instalação Local
1. Faça o download dos arquivos do projeto
2. Coloque o arquivo Excel na mesma pasta (opcional)
3. Abra o arquivo `index.html` em seu navegador
4. O dashboard estará pronto para uso

### Configuração Personalizada
Para personalizar o dashboard:
1. Edite as cores no CSS (variáveis de cor no início do arquivo)
2. Ajuste os filtros conforme suas necessidades
3. Modifique os campos das tabelas se necessário

## 🚀 Funcionalidades Avançadas

### Carregamento Automático
- O sistema tenta carregar automaticamente o arquivo `DASHBOAR PARA DESENVOLVIMENTO 270525.xlsx`
- Se não encontrado, exibe uma mensagem de boas-vindas

### Processamento Inteligente
- Tratamento automático de dados vazios ou inválidos
- Conversão automática de tipos de dados
- Formatação adequada de datas, números e moedas

### Performance Otimizada
- Renderização eficiente de grandes volumes de dados
- Gráficos otimizados para performance
- Filtros com aplicação em tempo real

## 🐛 Solução de Problemas

### Problemas Comuns

**Arquivo não carrega:**
- Verifique se o arquivo está no formato Excel (.xlsx ou .xls)
- Confirme se as abas têm os nomes corretos
- Verifique se há dados nas planilhas

**Gráficos não aparecem:**
- Atualize a página
- Verifique se JavaScript está habilitado
- Confirme se há dados válidos no arquivo

**Dados incorretos:**
- Verifique a estrutura das colunas no Excel
- Confirme se as datas estão no formato correto
- Verifique se os valores numéricos não contêm texto

## 👤 Desenvolvedor

**Leandro Leal**
- Desenvolvido em 2025
- Especialista em dashboards e análise de dados

## 📄 Licença

Este projeto está licenciado sob a Licença MIT - veja o arquivo LICENSE para detalhes.

## 🔮 Próximas Funcionalidades

- [ ] Exportação de relatórios em PDF
- [ ] Integração com APIs externas
- [ ] Salvamento de configurações personalizadas
- [ ] Alertas e notificações automáticas
- [ ] Modo escuro/claro
- [ ] Dashboard em tempo real com WebSockets

## 🤝 Contribuindo

Contribuições são bem-vindas! Para contribuir:
1. Faça um fork do projeto
2. Crie uma branch para sua feature (`git checkout -b feature/AmazingFeature`)
3. Commit suas mudanças (`git commit -m 'Add some AmazingFeature'`)
4. Push para a branch (`git push origin feature/AmazingFeature`)
5. Abra um Pull Request

## 📞 Suporte

Para suporte técnico ou dúvidas sobre o dashboard, entre em contato através dos canais oficiais da Bomix.

---

**Dashboard Bomix** - Transformando dados em insights para decisões inteligentes. 🚀