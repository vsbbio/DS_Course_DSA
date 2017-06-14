Antes de começar o processo de análise, procure compreender o conjunto de dados que possui em mãos:

1. Como as variáveis e as observações estão distribuidas @dataset
2. Que tipo de dados temos em mãos
3. Como esses dados se relacionam

Pipeline:

## 1. print(df.head())
## 2. print(df.describe())
## 3. Gráficos:

  * Histograma:
      df.risk_rate.hist(bins=100)
      plt.xlabel("xlabel")
      plt.ylabel("ylabel")
      plt.title("Título")
      plt.show()

  * Pizza:
      labels = dfb.score_1.value_counts().index
      num = len(dfb.score_1.value_counts().index)
      sizes = dfb.score_1.value_counts()
      fig1, ax1 = plt.subplots()
      ax1.pie(sizes, autopct="%1.1f%%",startangle=10, explode=[0.0](vezes)num)
      ax1.axis("equal")
      ax1.legend(labels, bbox_to_anchor=(1.25,1))
      plt.show()

 * Barra Crosstab:
      dfc = dfb.copy()
      bins = [0,0.1,0.2,0.3,0.4,0.5,0.6,0.7,0.8,0.9]

      dfc.risk_rate = pd.cut(dfc.risk_rate, bins, labels=["1","2","3","4","5","6","7","8","9"])

      dfc2 = pd.crosstab(dfc.risk_rate, dfc.default).apply(lambda x:x/x.sum(), axis=1)

      ax1 = dfc2.plot(kind="bar", stacked=True, title="Default x Income")

      fig1, labels = ax1.get_legend_handles_labels()
      ax1.legend(fig1, labels, bbox_to_anchor=(1.25,1))

 * Regressão Linear

     dfc = dfb.copy()

    col = "risk_rate"
    col2 = "score_6"

    dfc = dfc.dropna(subset=[col, col2])
    x = dfc[col]
    y = dfc[col2]

    m, b = np.polyfit(x, y, 1)
    plt.plot(x, y,".", color="green")
    plt.plot(x, m*x+b, '-', color="black")
    plt.xlabel(x.name)
    plt.ylabel(y.name)
    plt.show()
