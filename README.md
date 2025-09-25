import matplotlib.pyplot as plt

# dados
x  =[1, 2, 3, 4, 5]
y = [2, 4, 1, 3, 5]

# criar dois subplots (1 linha, 2 colunas)
fig, axes = plt.subplots(1, 2, figsize=(10, 4))

# Plotar o gráfico de linha no primeiro subplot
axes[0].plot(x, y)
axes[0].set_xlabel('Eixo X')
axes[0].set_ylabel('Eixo Y')
axes[0].set_title('Gráfico de Linha')

# Plotar o gráfico de barras no segundo subplot
axes[1].bar(x, y)
axes[1].set_xlabel('Eixo X')
axes[1].set_ylabel('Eixo Y')
axes[1].set_title('Gráfico de Barras')

# Ajustar o layout para evitar sobreposição
plt.tight_layout()

# Mostrar os gráficos
plt.show()
