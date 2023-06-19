import pandas as pd

# Exercício 1

# df = pd.read_csv('https://raw.githubusercontent.com/Igfernandes/bigdata-av3/main/world_alcohol.csv')
# Observação, está bloquenado o acesso da URL com error 403. Estarei colocando no meu repositório no github por isso.

# print(df)
# Exercício 1 - A
# df.groupby(['Beverage Types']).get_group('Beer')

# Exercício 1 - B
# df.groupby(['Year','WHO region']).groups

# Exercício 1 - C
# df.groupby(['WHO region', 'Country']).size()
# df.groupby('Beverage Types').get_group('Beer')['Display Value'].sum();

# Exercicio 1 - D
# valuesOfBeer = df.groupby(['Beverage Types']).get_group('Beer')['Display Value']
# print(valuesOfBeer.mean())
# print(valuesOfBeer.median())
# print(valuesOfBeer.mode())
# print(valuesOfBeer.describe())
# valuesOfBeer.plot(kind='line')

# Exercício 1 - E
# colBeer = df.groupby(['Beverage Types']).get_group('Beer')[df['Year'] == 1985]
# print(colBeer)
# colRegion = df['WHO region'][df['Display Value'] > 4]
# print(colRegion)


# =================================================//==========================//=============================//==========

# Exercício 2

df = pd.read_csv('https://raw.githubusercontent.com/Igfernandes/bigdata-av3/main/cursos-prouni.csv');

# Exercício 2 - A:
# print(df.replace(to_replace=np.nan, value="0,0"))
# df = df.replace(to_replace=np.nan, value="0,0");

# Exercício 2 - B:
# print(df.groupby(['grau']).sum())

# Exercício 2 - C:
#df.groupby('curso_busca').get_group(('Medicina', 'Pedagogia', 'Matemática'))

# Exercício 2 - D:
# df.groupby('uf_busca').mean()

# Exercício 2 - E:
# df.groupby('grau').get_group('Tecnológico')

# Exercício 2 - F:
# df.drop('cidade_filtro', inplace=True, axis=1)

# Exercício 2 - G:
# df.groupby('curso_busca').get_group('Medicina')['mensalidade'].mean()

# Exercício 2 - H:
# print(df.groupby(['turno']).get_group('Integral').mean())

# Exercício 2 - I:
# df.groupby('grau').get_group('Bacharelado')['nota_integral_ampla'].describe()

# Exercício 2 - J:
# df.groupby('grau')['nota_integral_cotas'].value_counts().plot(kind='line')
