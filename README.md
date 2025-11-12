[README.txt](https://github.com/user-attachments/files/23508788/README.txt)
Calculadora de Horas Extras - Azepel
📋 Descrição
Aplicação web mobile-first para cálculo de horas extras dos funcionários da Azepel. Permite que qualquer funcionário calcule o valor das suas horas extras de forma rápida, simples e segura, com opção de compartilhamento via WhatsApp.
---
🚀 Como Usar
Para Funcionários (Acesso via Link)
Clique no link fornecido pela empresa ou acesse direto no navegador
Preencha os campos solicitados:
Salário bruto mensal: informe seu salário em reais
Horas extras: escolha uma das duas opções:
Informar o total de horas extras diretamente (HH:MM)
Informar horário de entrada e saída para cálculo automático
Tipo de hora extra: selecione entre 60% (normal) ou 100% (domingo/feriado)
DSR (opcional): marque se deseja incluir o descanso semanal remunerado e informe:
Dias úteis do mês
Domingos e feriados do mês
Clique em "Calcular"
Visualize o resultado detalhado com:
Valor da hora normal
Valor da hora extra
Total de horas extras
Valor do DSR (se aplicável)
Valor total a receber
Detalhamento completo do cálculo
(Opcional) Clique em "Compartilhar no WhatsApp" para enviar o resultado
---
💻 Requisitos Técnicos
Navegador web moderno (Chrome, Firefox, Safari, Edge)
Acesso à internet
Para uso no celular: qualquer smartphone com navegador
---
📊 Fórmulas Utilizadas
Cálculo da Hora Normal
```
Valor Hora Normal = Salário Mensal ÷ 220 horas
```
Cálculo da Hora Extra
```
Valor Hora Extra = Valor Hora Normal × (1 + Percentual/100)
```
Exemplo com 60%:
```
Valor Hora Extra = R$ 13,64 × 1,60 = R$ 21,82
```
Cálculo Total de Horas Extras
```
Total HE = Quantidade de Horas Extras × Valor Hora Extra
```
Cálculo do DSR (se incluído)
```
DSR = (Total de Horas Extras) ÷ Dias Úteis × (Domingos + Feriados)
```
Total a Receber
```
Total = Total de Horas Extras + DSR (se aplicável)
```
---
ℹ️ Informações Importantes
Carga Horária
Carga semanal: 44 horas (8:48 por dia)
Carga mensal: 220 horas (considerando 5 semanas por mês)
Percentuais de Hora Extra
60%: hora extra normal (dias úteis)
100%: hora extra domingo/feriado
Sobre o DSR
DSR é o valor do descanso semanal remunerado (domingos/feriados)
É opcional no cálculo, mas impacta no valor final a receber
Caso deixe em branco, uma aviso será exibido
---
🛠️ Instalação e Deploy
Opção 1: Deploy via GitHub + Vercel (Recomendado)
Criar repositório no GitHub:
Acesse github.com
Clique em "New repository"
Nome: `calc-horas-extras`
Marque como "Public"
Faça upload do arquivo `index.html`
Fazer deploy no Vercel:
Acesse vercel.com
Clique em "Sign Up" e escolha "Continue with GitHub"
Clique em "Import Git Repository"
Selecione o repositório `calc-horas-extras`
Clique em "Deploy"
Aguarde e acesse seu link (ex: `https://calc-horas-extras.vercel.app`)
Opção 2: Deploy via Vercel CLI
```bash
npm i -g vercel
vercel --prod
```
Opção 3: Usar Localmente (sem internet)
Baixe o arquivo `index.html`
Abra no navegador (duplo clique ou arraste para o navegador)
Use normalmente (funciona offline após carregar)
---
✅ Validações
A aplicação valida automaticamente:
✓ Valor de salário deve ser maior que zero
✓ Horários devem estar no formato HH:MM
✓ Horário de saída deve ser após horário de entrada
✓ Dias úteis deve estar entre 1 e 31
✓ Domingos/Feriados deve estar entre 1 e 31
✓ Todos os campos obrigatórios devem ser preenchidos
Mensagens de erro claras indicarão qualquer problema.
---
📱 WhatsApp
Ao clicar em "Compartilhar no WhatsApp":
A calculadora prepara uma mensagem formatada com os resultados
O WhatsApp Web abre automaticamente
Você escolhe o contato/grupo para enviar
A mensagem já vem pronta (não é editável)
Exemplo de mensagem:
```
Cálculo de Horas Extras
Salário base: R$ 3.000,00
Horas extras (60%): 20:00
Valor HE: R$ 436,36
DSR: R$ 72,73
Total a receber: R$ 509,09
```
---
🎨 Design
Otimizado para celular (mobile-first)
Interface limpa e intuitiva
Cores institucionais Azepel
Fontes legíveis
Botões grandes e fáceis de clicar
---
🔒 Privacidade e Segurança
✓ Sem armazenamento de dados: todos os cálculos são feitos localmente no navegador
✓ Sem banco de dados: nenhuma informação é enviada para servidor
✓ Sem cookies de rastreamento: apenas cookies técnicos necessários
✓ Os dados são processados apenas na sua máquina
---
📞 Suporte
Em caso de dúvidas ou problemas:
Verifique se está usando navegador atualizado
Tente limpar o cache do navegador (Ctrl+Shift+Del)
Teste em outro navegador
Contate o departamento de TI/RH da empresa
---
📝 Notas Técnicas
Linguagem: HTML5 + CSS3 + JavaScript (Vanilla)
Hospedagem: Vercel (gratuita e escalável)
Framework: Nenhum (código puro para máxima compatibilidade)
Responsividade: Mobile-first, funciona em qualquer tela
Performance: Página leve (<50KB) e rápida
---
📅 Histórico de Versões
v1.0 - 12/11/2025
Lançamento inicial
Cálculo de horas extras com 2 opções de entrada
Percentuais de 60% e 100%
Cálculo de DSR opcional
Exportação para WhatsApp
Design mobile-first responsivo
---
📄 Licença
Desenvolvido para uso interno da Azepel.
---
Desenvolvido com ❤️ para Azepel
