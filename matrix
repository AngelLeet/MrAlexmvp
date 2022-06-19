#include <stdio.h>
#include <stdlib.h>


void matrix_1(int*** matrix, int*** matrix_2, int* N, int* M, int* L, int* K);
void umno(int** matrix, int** matrix_2, int M, int L);
void output(int** matrix, int N, int M, int** matrix_2, int L, int K);

int main() {
	int N, M, K, L;
	int** matrix;
	int** matrix_2;
	matrix_1(&matrix, &matrix_2, &N, &M, &L, &K);
	output(matrix, N, M, matrix_2, L, K);
	umno(matrix, matrix_2, M, L);

}


void matrix_1(int*** matrix, int*** matrix_2, int* N, int* M, int* L, int* K) {
	int k = 0;
	if (scanf("%d %d", N, M) != 1) {
		(*matrix) = malloc((*N) * sizeof(int*));
			for (int i = 0; i < (*N); i++){
				(*matrix)[i] =malloc((*M) * sizeof(int));
			}

		for (int i = 0; i < (*N); i++){
			for (int j = 0; j < (*M); j++){
				scanf("%d", &k);
				(*matrix)[i][j] = k;
			}
		}
	if (scanf("%d %d", L, K) != 1) {
		(*matrix_2) = malloc((*L) * sizeof(int*));
		for (int i = 0; i < (*L); i++){
			(*matrix_2)[i] = malloc((*K) * sizeof(int));
		}

		for (int i = 0; i < (*L); i++){
			for (int j = 0; j < (*K); j++) {
				scanf("%d", &(*matrix_2)[i][j]);
			}
			}
		}
	}
	}


void output(int** matrix, int N, int M, int** matrix_2, int L, int K) {
	for (int i = 0; i < N; i++){
		for (int j = 0; j < M; j++){
			printf("%d ", matrix[i][j]);
		}
		printf("\n");
	}
	for (int i = 0; i < L; i++){
		for (int j = 0; j < K; j++){
			printf("%d ", matrix_2[i][j]);
		}
		printf("\n");
	}
}

void umno(int** matrix, int** matrix_2, int M, int L){
	int kol[M][L];

	int sum = 0;
	if (M == L) {
		for (int k = 0; k < M - 1; k++)
			
			for (int i = 0; i < M-1; i++) {
				
				for (int j = 0; j < L; j++) {

					sum = sum + (matrix[k][j] * matrix_2[j][i]);
					//printf("%d ", sum);
					
				}

				kol[i][k] = sum;
				sum = 0;


			}



	for (int i = 0; i < L - 1 ; i++){
		for (int j = 0; j < M - 1 ; j++) {
			printf("%d ", kol[i][j]);
		}
		printf("\n");
	}


	} else {
		printf("n/a");
	}
}
