# Reforma Tributária Simulator

Simulador da transição para **CBS, IBS e Imposto Seletivo** (EC 132/2023 e LC 214/2025), feito para o departamento fiscal.

**Abrir o app:** https://amenta94.github.io/reforma-tributaria-simulator/

## O que faz

- Importa XML de NF-e, CT-e e NFS-e (Nacional e ABRASF), EFD ICMS/IPI (vários arquivos da mesma raiz de CNPJ) e planilha de operações.
- Classifica cada operação (CST IBS/CBS e cClassTrib) pelo motor de regras, com a situação do enquadramento: Confirmado, Conferir, Escolher enquadramento ou Sem fundamento.
- Simula CBS, IBS e IS de 2026 a 2033, compara a carga atual (ICMS, IPI, PIS/COFINS, ISS) com a reforma, estima créditos por fornecedor e gera relatórios em PDF e Excel.
- Inclui a tabela de cClassTrib (Portal SVRS), a NCM e a NBS 2.0 embutidas.

## Privacidade

Todo o processamento acontece **no navegador**. Nenhum XML, SPED ou planilha é enviado para servidor. As validações ficam salvas no próprio navegador (localStorage) e podem ser exportadas em **Configurações → Backup das validações**.

## Instalar como aplicativo

No Chrome ou Edge, abra o link e use **Instalar aplicativo** na barra de endereço. Depois de aberto uma vez, o app funciona offline.

## Atualizar

Substitua os arquivos deste repositório pela nova versão (principalmente `index.html`, `sw.js` e `versao.json`). Quem estiver com o app aberto vê o aviso **"Nova versão disponível"**.

## Aviso

Ferramenta de apoio à análise. Alíquotas de 2027 em diante são premissas editáveis; enquadramentos sem fundamento confirmado aparecem como **NECESSITA DE VALIDAÇÃO NA LEGISLAÇÃO/TABELA OFICIAL VIGENTE**. Confira sempre o texto legal e a tabela oficial vigente antes de aplicar.
