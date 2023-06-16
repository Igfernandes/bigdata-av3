import pandas as pd

index = 0;
df = pd.read_csv('https://raw.githubusercontent.com/Igfernandes/bigdata-av3/main/cursos-prouni.csv.csv');

# Exercício 2 - A:
# print(df.replace(to_replace=np.nan, value="0,0"))
df = df.replace(to_replace=np.nan, value="0,0");

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

# Exercício 2 - G: INCOMPLETO - NÃO ESTÁ FUNCIONANDO O GET_GROUP
# df.groupby('curso_busca').get_group('Medicina')['mensalidade'].mean()

# Exercício 2 - H:  INCOMPLETO
# df.groupby('turno')..mean()

# Exercício 2 - I: 
# df.groupby('grau').get_group('Bacharelado')['nota_integral_ampla'].describe()

# Exercício 2 - J: 
# df.groupby('grau')['nota_integral_cotas'].value_counts().plot(kind='line')
