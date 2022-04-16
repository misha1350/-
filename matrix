def ShowMatrix(matrix):
	for x in range(size):
		for y in range(size):
			print(matrix[x][y], end = " ")
		print("")

def EnterMatrix(size):
	matrix = [[0 for x in range (size)] for y in range(size)]
	for x in range(size):
		for y in range(size):
			t = int(input("Введите значения (20000 - выход): "))
			if (t != 20000):
				matrix[x][y] = t
				ShowMatrix(matrix)
			else:
				print("Выходим из матрицы...")
				return matrix
	return matrix

def MultiplyMatrices(matrix_one, matrix_two):
	multiplied_matrix = [[0 for x in range (size)] for y in range(size)]
	for row in range (size):
		for column in range (size):
			for inner in range (size):
				multiplied_matrix[row][column] += matrix_one[row][inner] * matrix_two[inner][column]
	return multiplied_matrix
		

size = int(input("Введите размер матрицы: "))
matrix_one = EnterMatrix(size)
matrix_two = EnterMatrix(size)
multiplied_matrix = MultiplyMatrices(matrix_one, matrix_two)
ShowMatrix(multiplied_matrix)