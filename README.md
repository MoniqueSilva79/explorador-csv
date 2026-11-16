# 📊 Explorador de CSV

**🔗 Demo ao vivo: https://moniquesilva79.github.io/explorador-csv/**

Arraste um CSV e receba o **perfil dos dados** na hora: tipo de cada coluna, valores ausentes, linhas duplicadas, estatísticas descritivas, histogramas, valores mais frequentes e matriz de correlação. Os dados não saem do seu computador.

## 🎯 Problema que resolve
Antes de qualquer análise ou modelo de IA, é preciso entender os dados: o que é número, o que é texto, onde há buracos e o que se relaciona com o quê. Este explorador faz esse diagnóstico inicial em segundos, sem instalar Python nem subir a planilha em serviço nenhum.

## ✨ Funcionalidades
- Leitor de CSV próprio (aspas, separador vírgula ou ponto e vírgula, BOM)
- Números no formato brasileiro (1.234,56 e R$) e datas DD/MM/AAAA ou AAAA-MM-DD
- Detecção automática de tipo: numérica, data ou categoria
- Estatísticas (média, mediana, desvio, mínimo e máximo), histogramas e top 5 valores
- Correlação de Pearson com mapa de calor
- Conjunto de dados de exemplo (clientes de fibra fictícios)

## 🧮 Como o cálculo funciona
```
Correlação de Pearson: r = Σ(x − x̄)(y − ȳ) ÷ √(Σ(x − x̄)² × Σ(y − ȳ)²)
Mediana e quartis por interpolação linear
```

## 🧰 Tecnologias
HTML, CSS e JavaScript puros, sem frameworks, sem dependências e sem servidor. Publicado no GitHub Pages.

## 🚀 Como rodar localmente
```bash
git clone https://github.com/MoniqueSilva79/explorador-csv.git
cd explorador-csv
# abra o index.html no navegador, ou sirva a pasta:
python -m http.server 8000   # e acesse http://localhost:8000
```

## ⚠️ Limitações
Pensado para arquivos de até algumas dezenas de MB. Arquivos maiores podem deixar o navegador lento.

## 🗺️ Próximos passos
- [ ] Gráfico de dispersão ao clicar em uma célula da correlação
- [ ] Detecção de outliers
- [ ] Exportar o relatório em HTML

---
Projeto autoral de **Monique da Silva Cruz**: [LinkedIn](https://www.linkedin.com/in/moniquesilva-cloud-ti-projetos-latam) · [outros projetos](https://github.com/MoniqueSilva79)
